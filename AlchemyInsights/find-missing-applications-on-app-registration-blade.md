---
title: Suchen fehlender Anwendungen auf dem Blatt "App-Registrierung"
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
- "9004352"
- "9654"
ms.openlocfilehash: 0a00948ef99486b3cfae219dd9bc338349a376dc
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65720285"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Suchen fehlender Anwendungen auf dem Blatt "App-Registrierung"

1. Anwendungen wurden im App-Registrierungsportal nicht gefunden.

    Wenn es sich bei einer Anwendung um eine Mehrinstanzenanwendung handelt und sie in einem anderen Mandanten registriert wurde, wird sie nicht unter dem Blatt "App-Registrierung" angezeigt. Möglicherweise finden Sie es jedoch unter Enterprise Blatt "Anwendungen", nachdem auf das Blatt zugegriffen wurde (nachdem die Zustimmung erteilt wurde) und der Dienstprinzipal in Ihrem Mandanten erstellt wurde. Weitere Informationen finden Sie [unter Apps & Dienstprinzipale in Azure AD – Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Apps können nicht auf dem Blatt "App-Registrierung" angezeigt werden, obwohl Sie ein Administrator sind.

    Stellen Sie sicher, dass Sie sich im richtigen Verzeichnis auf dem Azure-Portal befinden.
3. Meine Anwendung wird nicht unter Enterprise Blatt "Anwendungen" aufgeführt, wird aber angezeigt, wenn ich den PowerShell-Befehl abfrage.

    Manchmal wird die Anwendung nach dem Löschen aus dem Azure-Portal nicht im Portal angezeigt, aber möglicherweise nicht vollständig gelöscht. Weitere Informationen finden Sie unter:
    - Mithilfe des **Powershell-Befehls "Get-AzureADDeletedApplication**" können Sie die Liste der zuvor gelöschten Anwendungen abrufen und sehen, ob die Anwendung in der Liste angezeigt wird. Weitere Informationen finden Sie unter [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Wenn Sie die Anwendung vollständig entfernen möchten, können Sie Folgendes in PowerShell ausprobieren: **Remove-AzureADApplication -ObjectId**. Weitere Informationen finden Sie unter [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Alternativ können Sie versuchen, die gelöschte Anwendung mit dem folgenden Powershell-Befehl **wiederherzustellen: AzureADDeletedApplication -ObjectId wiederherstellen**. Weitere Informationen finden Sie unter [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Es wurde keine Liste aller vorinstallierten Unternehmensanwendungen in meinem neuen Azure-Mandanten gefunden.

    In Azure AD sind standardmäßig keine vorinstallierten Unternehmensanwendungen vorhanden. Sie müssen sie manuell über die Option "Neue Anwendung" hinzufügen, indem Sie sie aus dem Azure AD-Katalog durchsuchen oder eine Nicht-Kataloganwendung hinzufügen. Weitere Informationen finden Sie in der [Schnellstartanleitung: Hinzufügen einer Anwendung zu Ihrem Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).
    Wenn Sie ein globaler Administrator sind, können Sie ganz einfach mit dem [Microsoft 365 App-Startfeld](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher) auf Ihre Apps zugreifen.
5. Meine Apps können nicht über Meine Apps Portal gefunden werden.

    Stellen Sie sicher, dass Apps nicht auf Meine Apps Sammlungsseite ausgeblendet sind. Weitere Informationen finden Sie [unter Sammlungen (Vorschau) im Meine Apps-Portal – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Informationen zum Starten von Apps über das Meine Apps-Portal finden [Sie unter "Suchen & Verwenden von Apps im Meine Apps-Portal – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)".
7. Office 365 Mover-App wird nach der Installation nicht auf Enterprise Blatt "Anwendungen" angezeigt.

    Die Anwendung "Office 365 Mover" ist eine mehrinstanzenfähige App, die AAD nicht über den Abschnitt "Kataloganwendungen" unter Enterprise App-Registrierung hinzugefügt werden muss. Um auf Office 365 Mover-App zuzugreifen, melden Sie sich einfach bei der App an, und sie fordert die Zustimmung des Benutzers für die Berechtigungen an. Sobald der Benutzer die Zustimmung erteilt hat, wird diese App dem Mandanten automatisch mit der E-Mail-ID hinzugefügt, die Sie angemeldet haben.

    Nachdem Sie sich bei der Anwendung angemeldet haben, sollten Sie in der Lage sein, den Eintrag dieser Anwendung unter dem Blatt Enterprise Anwendungen in AAD zu finden. Sie müssen nach dieser Anwendung suchen, indem Sie entweder den vollständigen Namen eingeben, d. h. "Office 365 Mover" oder einfach "Office" suchen und die App auflisten. Weitere Informationen finden Sie [unter Office 365 Mover sagt, dass es bereits installiert ist, aber nicht im Enterprise Anwendungskatalog aufgeführt ist](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).
8. [Schnellstart: Die Liste der Anwendungen, die Ihren Azure Active Directory (Azure AD)-Mandanten für die Identitätsverwaltung verwenden](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal), zeigt Ihnen, wie Sie die Anwendungen anzeigen, die auch als Apps bezeichnet werden, die bereits für die Verwendung Ihres Azure AD-Mandanten als Identitätsanbieter (IdP) eingerichtet sind.
9. [Die Problembehandlung bei häufig auftretenden Problemen beim Hinzufügen oder Entfernen einer Anwendung zu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) hilft Ihnen, die häufig auftretenden Probleme zu verstehen, mit der Personen beim Anzeigen von Apps in Azure Active Directory konfrontiert sind.
