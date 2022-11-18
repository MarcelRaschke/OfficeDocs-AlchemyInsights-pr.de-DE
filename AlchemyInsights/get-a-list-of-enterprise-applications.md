---
title: Abrufen einer Liste von Unternehmensanwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: fe87a01650203713b59981cc60ae502a601f2f80
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66311076"
---
# <a name="get-a-list-of-enterprise-applications"></a>Abrufen einer Liste von Unternehmensanwendungen

1. Informationen zum **Abrufen einer Liste von Unternehmensanwendungen** (alle Anwendungen oder gefiltert nach Anzeigename, ID, Bezeichner-URIs usw.) über den Powershell-Befehl finden [Sie unter Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Informationen zum Abrufen einer Liste von Dienstprinzipalobjekten (alle Objekte oder gefiltert nach ID) über den [Powershell-Befehl finden Sie unter Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Wenn Sie **eine Liste der SAML-konfigurierten Apps abrufen möchten, können Ihnen die folgenden PowerShell-Skripts** helfen:

    Jede Anwendung, sei es eine OAuth-App oder SAML-App (sowohl Galerie- als auch Nicht-Katalog-Apps), würde zwei Objekte in AAD erstellen, wenn die Registrierung erfolgt. Eines wird als Application-Objekt und das andere als Dienstprinzipalobjekt bezeichnet. Wenn Sie die Eigenschaften eines Dienstprinzipalobjekts mithilfe von PowerShell abbilden, würden Sie feststellen, dass jeder Anwendung eine bestimmte Anzahl von Tags zugeordnet ist:

    - OAuth-Apps hätten ein Tag namens "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Katalog-SAML-Apps hätten ein Tag namens "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Nicht-Katalog-SAML-Apps hätten ein Tag namens "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Daher können Sie diese Tags verwenden und herausfinden, um welche Art von App es sich handelt. Das Tag "**WindowsAzureActiveDirectoryIntegratedApp**" ist für alle Arten von Apps üblich. Sie können den folgenden Codeausschnitt verwenden, um alle SAML-Apps (sowohl Katalog als auch Nicht-Katalog) auflisten:

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Weitere Informationen finden Sie unter [Identifizieren von SAML-fähigen Apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Nur Webanwendungen suchen und auflisten**: Verwenden Sie den folgenden Befehl, um alle Azure AD-Anwendungen mit dem Anwendungstyp "Web App/API" abzurufen.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Nur native Anwendungen suchen und auflisten**: Führen Sie den folgenden Befehl aus, um alle systemeigenen Clientanwendungen (Desktop-/Mobile-Geräte) abzurufen.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Alle registrierten Azure AD-Anwendungsdetails nach CSV exportieren**: Der folgende Befehl exportiert alle Azure AD-Apps mit den erforderlichen Details in die CSV-Datei:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Exportieren einer Liste nicht verwendeter Azure-Apps** – Überwachungsbericht

    Azure AD kann Anwendungsprotokolle nur für bis zu 30 Tage anzeigen, sofern Sie über eine Azure AD Premium-Lizenz verfügen.
    Sie haben zwei Möglichkeiten, die Daten länger als 30 Tage aufzubewahren. Sie können die [Azure AD Reporting-APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) verwenden, um die Daten programmgesteuert abzurufen und in einer Datenbank zu speichern. Alternativ können Sie Überwachungsprotokolle in ein SIEM-System eines Drittanbieters integrieren.

    Sie können auch die App-Liste für alle Anwendungen und im Besitz befindlichen Anwendungen unter Azure Active Directory>App-Registrierungen herunterladen>>Alle Anwendungen/Eigenen Anwendungen herunterladen.

    Eine Liste der Anwendungen über MS Graph finden Sie unter [Listenanwendungen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) und [Anwendungsressourcentyp – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
