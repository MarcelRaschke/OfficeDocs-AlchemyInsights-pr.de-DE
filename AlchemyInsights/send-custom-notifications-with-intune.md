---
title: Senden von benutzerdefinierten Benachrichtigungen mit Intune
ms.author: brenduns
author: brenduns
manager: dougeby
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 01d78c5b052e59f9852bd808b05b8f4545377213
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66291403"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>So senden Sie benutzerdefinierte Benachrichtigungen an Benutzer von verwalteten iOS- und Android-Geräten

Benutzerdefinierte Benachrichtigungen für Intune werden von der Unternehmensportal-App auf dem Gerät eines Benutzers verarbeitet. Die App erstellt dann die Pushbenachrichtigung auf diesem Gerät.

Die folgenden Gerätevoraussetzungen unterstützen den Empfang von benutzerdefinierten Benachrichtigungen, und die App kann dann die Pushbenachrichtigung erstellen:

- Auf dem Gerät muss die Unternehmensportal-App installiert sein.  

- Das Gerät muss zulassen, dass die Unternehmensportal-App Pushbenachrichtigungen sendet. Wenn die App installiert oder aktualisiert wird, wird der Benutzer aufgefordert, Benachrichtigungen zuzulassen.

- Auf Android-Geräten muss Google Play Services installiert sein.

- Das Gerät muss bei Intune registriert sein.

Weitere Informationen, einschließlich des Sendens einer Nachricht, finden Sie in der [Featuredokumentation](https://docs.microsoft.com/intune/custom-notifications).
