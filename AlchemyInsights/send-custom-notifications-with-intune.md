---
title: Senden von benutzerdefinierten Benachrichtigungen mit Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: a7b1e4e363b586b36f9777396ec97ed37c894618
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65721653"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>So senden Sie benutzerdefinierte Benachrichtigungen an die Benutzer von verwalteten iOS und Android Geräten

Benutzerdefinierte Benachrichtigungen für Intune werden von der Unternehmensportal-App auf dem Gerät eines Benutzers verarbeitet. Die App erstellt dann die Pushbenachrichtigung auf diesem Gerät.

Die folgenden Gerätevoraussetzungen unterstützen den Empfang von benutzerdefinierten Benachrichtigungen, und die App kann dann die Pushbenachrichtigung erstellen:

- Auf dem Gerät muss die Unternehmensportal-App installiert sein.  

- Das Gerät muss zulassen, dass die Unternehmensportal-App Pushbenachrichtigungen sendet. Wenn die App installiert oder aktualisiert wird, wird der Benutzer aufgefordert, Benachrichtigungen zuzulassen.

- Android Geräte müssen Google Play Services installiert sein.

- Das Gerät muss bei Intune registriert sein.

Weitere Informationen, einschließlich des Sendens einer Nachricht, finden Sie in der [Featuredokumentation](https://docs.microsoft.com/intune/custom-notifications).
