---
title: Abrufen einer Liste von Enterprise-Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 52d575bd5e7bb18044cca68cf54b0a59ad845767
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63237471"
---
# <a name="get-a-list-of-enterprise-applications"></a>Abrufen einer Liste von Enterprise-Anwendungen

1. Informationen **zum Abrufen einer Liste von Unternehmensanwendungen** (alle Anwendungen oder gefiltert nach Anzeigename, ID, Bezeichner-URIs usw.) über den PowerShell-Befehl finden Sie unter ["Get-AzureADApplication (AzureAD)"](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Informationen zum Abrufen einer Liste von Dienstprinzipalobjekten (alle Objekte oder gefiltert nach ID) über den PowerShell-Befehl finden Sie unter [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Wenn Sie **eine Liste der konfigurierten SAML-Apps abrufen möchten, können Ihnen die folgenden PowerShell-Skripts** helfen:

    Jede Anwendung, sei es eine OAuth-App oder SAML-App (sowohl Katalog- als auch Nicht-Katalog-Apps), verfügt über zwei Objekte, die in AAD erstellt werden, wenn ihre Registrierung erfolgt. Eine wird als Application-Objekt und die andere als Dienstprinzipalobjekt bezeichnet. Wenn Sie die Eigenschaften eines Dienstprinzipalobjekts mithilfe von PowerShell abbilden, stellen Sie fest, dass jeder Anwendung eine bestimmte Anzahl von Tags zugeordnet ist, z. B.:

    - OAuth-Apps hätten das Tag "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Nicht-Katalog-SAML-Apps hätten ein Tag namens "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Daher können Sie diese Tags verwenden und herausfinden, um welche Art von App es sich handelt. Das Tag "**WindowsAzureActiveDirectoryIntegratedApp**" ist für alle Arten von Apps üblich. Mit dem folgenden Codeausschnitt können Sie alle SAML-Apps auflisten (sowohl im Katalog als auch nicht im Katalog):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Weitere Informationen finden Sie unter [Identifizieren von SAML-fähigen Apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Nur Webanwendungen suchen und auflisten**: Verwenden Sie den folgenden Befehl, um alle Azure AD Anwendungen mit dem Anwendungstyp "Web app/API" abzurufen.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Suchen und Auflisten systemeigener Anwendungen allein**: Führen Sie den folgenden Befehl aus, um alle nativen Clientanwendungen (Desktop-/Mobile-Gerät) abzurufen.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Exportieren Sie alle registrierten Azure AD Anwendungsdetails in CSV**: Mit dem folgenden Befehl werden alle Azure AD Apps mit den erforderlichen Details in die CSV-Datei exportiert:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Exportieren einer Liste nicht verwendeter Azure-Apps** – Überwachungsbericht

    Azure AD können Anwendungsprotokolle nur bis zu 30 Tage lang anzeigen, sofern Sie über Azure AD Premium Lizenz verfügen.
    Sie haben zwei Möglichkeiten, die Daten länger als 30 Tage aufzubewahren. Sie können die [Azure AD Berichterstellungs-APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) verwenden, um die Daten programmgesteuert abzurufen und in einer Datenbank zu speichern. Alternativ können Sie Überwachungsprotokolle in ein SIEM-System eines Drittanbieters integrieren.

    Sie können auch die App-Liste für alle Anwendungen und eigenen Anwendungen unter Azure Active Directory>App-Registrierungen>Herunterladen>Alle Anwendungen/Anwendungen im Besitz herunterladen.

    Informationen zum Abrufen einer Liste von Anwendungen über MS Graph finden Sie unter ["Anwendungen auflisten" – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) und [Anwendungsressourcentyp – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
