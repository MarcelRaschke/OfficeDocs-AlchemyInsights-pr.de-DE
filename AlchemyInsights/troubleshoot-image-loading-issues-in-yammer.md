---
title: Behandeln von Problemen beim Laden von Bildern in Yammer
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 78eea4cf0b1afcf9369fb20d1f7bb9b57c85f0aa
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61982239"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Behandeln von Problemen beim Laden von Bildern in Yammer

Wenn in Yammer Probleme mit Fotos und der Dateivorschau auftreten, können Sie diese beheben, indem Sie überprüfen, ob das Problem für alle Benutzer auftritt, ob es auf mobilen Geräten geschieht, und ob es beim Hochladen der Anlage reproduzierbar ist.  

**Probleme mit dem Profilfoto**  

Wenn sich Endbenutzer über Microsoft 365 bei Yammer anmelden, müssen sie ihr Profil einschließlich des Profilfotos ändern. Wenn Benutzer keine Profilupdates vornehmen dürfen, kann ein Administrator das Update für den Benutzer vornehmen. Weitere Informationen finden Sie unter [Anzeigen und Aktualisieren Ihres Profils in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Informationen zum Bearbeiten des Profils, einschließlich der Profilfotos, finden Sie unter [Ändern des Yammer-Profils und der Yammer-Einstellungen](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Aktualisierte Profilfotos werden anders synchronisiert als Profilattribute. Benutzer müssen sich anmelden, um eine Synchronisierung Ihres Profilfotos zu initiieren. Informationen finden Sie unter [Werden Benutzerprofilbilder aus Office 365 in Yammer aktualisiert?](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Informationen zum Benutzerlebenszyklus für Yammer finden Sie unter [Verwalten von Yammer-Benutzern über ihren gesamten Lebenszyklus in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Einzelheiten dazu, wie die Profilbildsynchronisierung in Microsoft 365 funktioniert, finden Sie unter [Informationen zur Profilbildsynchronisierung in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Probleme mit der Dokumentvorschau und der Miniaturansicht von Bildern**  

Wenn Dateien oder Bilder in Yammer gepostet werden, werden Vorschauoptionen möglicherweise aus den folgenden Gründen nicht angezeigt: 

- Die Datei ist beschädigt und kann nicht geöffnet verarbeitet.
- Die Datei wurde nicht kürzlich in SharePoint Online hochgeladen, oder Yammer verfügt aus anderen Gründen über ungültige Metadaten.
- URLs, die zum Laden der Vorschaubilder erforderlich sind, werden blockiert.
- Die Dateivorschau wurde vom Benutzer vor dem Posten entfernt.
- Ein Problem mit dem Dienst hat die Generierung einer Vorschau verhindert.

**Hinweis** Vorschauen für Links und Dateiuploads können sich anders verhalten. Links zu Dateien im Internet oder Links, für die eine zusätzliche Authentifizierung erforderlich ist, werden möglicherweise nicht ordnungsgemäß angezeigt.

Weitere Informationen hierzu finden Sie unter [Anfügen einer Datei oder eines Bilds an eine Yammer-Nachricht](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 