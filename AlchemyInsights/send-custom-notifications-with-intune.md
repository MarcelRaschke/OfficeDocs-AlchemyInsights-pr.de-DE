---
title: Senden von benutzerdefinierten Benachrichtigungen mit Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: fe42a8cf4577b155ac7d65380bc28f14f1442a95
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62571339"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>So senden Sie benutzerdefinierte Benachrichtigungen an die Benutzer von verwalteten iOS- und Android-Geräten

Benutzerdefinierte Benachrichtigungen für Intune werden von der Unternehmensportal App auf dem Gerät eines Benutzers verarbeitet. Die App erstellt dann die Pushbenachrichtigung auf diesem Gerät.

Die folgenden Gerätevoraussetzungen unterstützen den Empfang von benutzerdefinierten Benachrichtigungen und damit die App dann die Pushbenachrichtigung erstellt:

- Auf dem Gerät muss die Unternehmensportal-App installiert sein.  

- Das Gerät muss zulassen, dass die Unternehmensportal-App Pushbenachrichtigungen sendet. Wenn die App installiert oder aktualisiert wird, fordert sie den Benutzer auf, Benachrichtigungen zuzulassen.

- Auf Android-Geräten muss Google Play Services installiert sein.

- Das Gerät muss bei Intune registriert sein.

Weitere Informationen, einschließlich des Sendens einer Nachricht, finden Sie in der [Featuredokumentation](https://docs.microsoft.com/intune/custom-notifications).
