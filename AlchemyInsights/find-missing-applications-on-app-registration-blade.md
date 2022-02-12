---
title: Suchen nach fehlenden Anwendungen auf dem Blatt "App-Registrierung"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 6cd940459095652c250c6f5b00ff43376bb8836b
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62710485"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Suchen nach fehlenden Anwendungen auf dem Blatt "App-Registrierung"

1. Anwendungen im App-Registrierungsportal können nicht gefunden werden.

    Wenn es sich bei einer Anwendung um eine mehrinstanzenfähige Anwendung handelt und sie in einem anderen Mandanten registriert wurde, wird sie nicht unter dem Blatt "App-Registrierung" angezeigt. Sie finden sie jedoch möglicherweise unter Enterprise Blatt "Anwendungen", sobald auf sie zugegriffen wurde (nach Zustimmung) und der Dienstprinzipal in Ihrem Mandanten erstellt wurde. Weitere Informationen finden Sie unter ["Apps & Dienstprinzipale" in Azure AD – Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Apps können im Blatt "App-Registrierung" nicht angezeigt werden, obwohl Sie Administrator sind.

    Stellen Sie sicher, dass Sie sich im Azure-Portal im richtigen Verzeichnis befinden.
3. Meine Anwendung wird nicht unter Enterprise Blatt "Anwendungen" aufgeführt, wird jedoch angezeigt, wenn ich den PowerShell-Befehl abfrage.

    Manchmal wird die Anwendung nach dem Löschen aus dem Azure-Portal nicht im Portal angezeigt, aber möglicherweise nicht vollständig gelöscht. Weitere Informationen finden Sie unter:
    - Mit dem **PowerShell-Befehl "Get-AzureADDeletedApplication**" können Sie die Liste der zuvor gelöschten Anwendungen abrufen und sehen, ob die Anwendung in der Liste angezeigt wird. Weitere Informationen finden Sie unter ["Get-AzureADDeletedApplication (AzureAD)"](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Wenn Sie die Anwendung vollständig entfernen möchten, können Sie Folgendes in PowerShell ausprobieren: **Remove-AzureADApplication -ObjectId**. Weitere Informationen finden Sie unter [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Alternativ können Sie versuchen, die gelöschte Anwendung mit dem folgenden PowerShell-Befehl **wiederherzustellen: AzureADDeletedApplication -ObjectId wiederherstellen**. Weitere Informationen finden Sie unter [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Liste aller vorinstallierten Unternehmensanwendungen in meinem neuen Azure-Mandanten kann nicht gefunden werden.

    In Azure AD sind standardmäßig keine vorinstallierten Unternehmensanwendungen vorhanden. Sie müssen sie manuell aus der Option "Neue Anwendung" hinzufügen, indem Sie sie aus Azure AD Katalog durchsuchen oder eine Anwendung hinzufügen, die nicht zum Katalog wird. Weitere Informationen finden Sie unter [Schnellstart: Hinzufügen einer Anwendung zu Ihrem Azure Active Directory(Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).
    Wenn Sie ein globaler Administrator sind, können Sie ganz einfach mit dem [Microsoft 365 App-Startprogramm](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher) auf Ihre Apps zugreifen.
5. Meine Apps können nicht über das Portal "Meine Apps" gefunden werden.

    Stellen Sie sicher, dass Apps nicht auf der Seite "Meine Apps"-Sammlung ausgeblendet sind. Weitere Informationen finden Sie [unter Sammlungen (Vorschau) im Portal "Meine Apps" – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Informationen zum Starten von Apps über das Portal "Meine Apps" finden [Sie unter Suchen & Verwenden von Apps im Portal "Meine Apps" – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Mover-App wird nach der Installation nicht auf dem Blatt Enterprise Anwendungen angezeigt.

    Die Anwendung "Office 365 Mover" ist eine mehrinstanzenfähige App, die nicht über den Abschnitt "Kataloganwendungen" unter Enterprise App-Registrierung AAD hinzugefügt werden muss. Um auf Office 365 Mover-App zuzugreifen, melden Sie sich einfach bei der App an, und sie fordert die Zustimmung des Benutzers für die Berechtigungen an. Nachdem der Benutzer die Zustimmung erteilt hat, wird diese App automatisch dem Mandanten mit der E-Mail-ID hinzugefügt, bei der Sie sich angemeldet haben.

    Nach der Anmeldung bei der Anwendung sollten Sie den Eintrag dieser Anwendung unter dem Blatt "Enterprise Anwendungen" in AAD finden können. Sie müssen nach dieser Anwendung suchen, indem Sie entweder den vollständigen Namen eingeben, d. h. "Office 365 Mover" oder einfach nach "Office" suchen und die App auflisten. Weitere Informationen finden Sie [unter Office 365 Mover gibt an, dass es bereits installiert ist, aber nicht im Enterprise Anwendungskatalog aufgeführt](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html) ist.
8. [Schnellstart: Anzeigen der Liste der Anwendungen, die Ihren Azure Active Directory (Azure AD)-Mandanten für die Identitätsverwaltung verwenden](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal), zeigt Ihnen, wie Sie die Anwendungen anzeigen, auch bekannt als Apps, die bereits für die Verwendung Ihres Azure AD Mandanten als Identitätsanbieter (IdP) eingerichtet sind.
9. [Problembehandlung beim Hinzufügen oder Entfernen einer Anwendung in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) hilft Ihnen, die allgemeinen Probleme zu verstehen, mit denen Benutzer beim Anzeigen von Apps in Azure Active Directory konfrontiert sind.
