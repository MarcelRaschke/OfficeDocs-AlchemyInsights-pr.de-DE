---
title: Problembehandlung beim Anmelden bei OneDrive
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: 1a34a2b1d0b131a8a8b431281b5c090e3a8894e7
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62615107"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>Problembehandlung beim Anmelden bei OneDrive

In diesem Artikel werden folgende Szenarien beschrieben:

- Fehlerbehebung beim Anmelden am OneDrive-Synchronisierungsclient
- Fehlerbehebung beim Anmelden an Ihrer OneDrive for Business-Website

**Fehlerbehebung beim Anmelden am OneDrive-Synchronisierungsclient**

- Schritte zum Beheben des Fehlercodes 0x004de40 finden Sie unter [Fehlercodecode 0x8004de40 bei der Anmeldung bei OneDrive](https://docs.microsoft.com/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive).
- Melden Sie sich bei OneDrive oder der SharePoint-Website an, indem Sie die Website besuchen, und klicken Sie auf die Schaltfläche **Synchronisieren** oben in der Menüleiste der Website. 
- Stellen Sie sicher, dass Sie sich bei OneDrive for Business anmelden, nicht bei OneDrive.com. Wenn die von Ihnen besuchte URL mit onedrive.live.com beginnt, ist dies nicht der Speicherort für Ihr OneDrive for Business. Eine einfache Möglichkeit, um sicherzustellen, dass Sie sich bei OneDrive for Business anmelden, ist dieser Link: https://portal.office.com/onedrive, dann verwenden Sie Ihr Geschäfts-, Schul- oder Unikonto, um sich anzumelden.
- Wenn Sie weiterhin Probleme haben, denken Sie daran, [OneDrive zurückzusetzen](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c).
- [Die Verknüpfung Ihres Kontos mit OneDrive aufheben](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1), melden Sie sich bei OneDrive oder der SharePoint-Website an, und klicken Sie dann auf die Schaltfläche **Synchronisieren** oben in der Menüleiste der Website. 

**Fehlerbehebung beim Anmelden an Ihrer OneDrive for Business-Website**

- Stellen Sie sicher, dass Sie sich bei OneDrive for Business anmelden, nicht bei OneDrive.com. Wenn die von Ihnen besuchte URL mit onedrive.live.com beginnt, ist dies nicht der Speicherort für Ihr OneDrive for Business. Eine einfache Möglichkeit, um sicherzustellen, dass Sie sich bei OneDrive for Business anmelden, ist dieser Link: https://portal.office.com/onedrive, dann verwenden Sie Ihr Geschäfts-, Schul- oder Unikonto, um sich anzumelden.
- Wenn Sie zu Ihrer Delve-Profilseite weitergeleitet werden, muss ein Microsoft 365-Administrator [den Benutzern die Berechtigung zum Erstellen ihrer OneDrive for Business-Website gewähren](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0).
- Testen Sie, ob Sie die OneDrive-Website mithilfe von [InPrivate-Browsen in Microsoft Edge](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) (oder einem ähnlichen Feature in einem anderen Browser) besuchen können.
    - Wenn das InPrivate-Browsen funktioniert, müssen Sie möglicherweise [Browserdaten in Microsoft Edge](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4) (oder einem ähnlichen Feature in einem anderen Browser) löschen.

**Problembehandlung beim Anmelden bei Office zum Synchronisieren mit OneDrive**

Wenn eine Fehlermeldung mit dem Inhalt **Upload blockiert**, **Anmelden, um diese Datei zu speichern** oder **Kopie speichern** angezeigt wird, müssen Sie [OneDrive aus den mit Office verbundenen Diensten möglicherweise entfernen und erneut verbinden](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8).

**Weitere Tipps zur Problembehandlung**

Wenn Sie ein globaler, Lizenz- oder Benutzeradministrator sind, [weisen Sie dem betroffenen Benutzer die richtige Lizenz zu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).

