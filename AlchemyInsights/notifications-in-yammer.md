---
title: Benachrichtigungen in Yammer
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: 5bd010a81405b27c6181d24b3c6a2a84bc129589
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62601491"
---
# <a name="notifications-in-yammer"></a>Benachrichtigungen in Yammer

Um Sie über neue Aktivitäten in relevanten Unterhaltungen zu informieren, [ sendet Yammer Benachrichtigungen](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) entweder per E-Mail oder – falls Sie Yammer auf Ihrem mobilen Gerät verwenden – über Pushbenachrichtigungen. Yammer sendet standardmäßig Benachrichtigungen für viele Arten von Aktivitäten in Ihrem Netzwerk gesendet. Benutzer können Ihre E-Mail-Einstellungen über die Yammer-Website aktualisieren, und Pushbenachrichtigungen werden über die mobile App konfiguriert. 

Yammer unterstützt jetzt auch [interaktive E-Mail-Nachrichten in Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Einige E-Mails (Kopie der Nachricht) werden in Outlook im Web interaktiv. Mit einem zukünftigen Update wird dies in anderen Versionen von Outlook bereitgestellt.

**Arten von Benachrichtigungen in Yammer**

- E-Mail-Nachrichten (Updates aus einer Gruppe, jemand lädt Sie zu einer Gruppe ein, Sie erhalten eine Nachricht in Ihrem Posteingang, usw.)
- Pushbenachrichtigungen (gesendet an mobile Geräte wenn Sie erwähnt werden, Sie erhalten eine Nachricht in Ihrem Posteingang, usw.)
- Desktoppopups (wenn die Yammer-Desktop-App installiert ist, werden Benachrichtigungen für Benutzer als Popupbenachrichtigungen angezeigt.)
- Glockenbenachrichtigungen (innerhalb der Yammer-Website werden Benutzern Benachrichtigungen für unterschiedliche Ereignisse angezeigt. Für diese Benachrichtigungen werden möglicherweise nicht immer entsprechende E-Mail-Nachrichten oder Pushbenachrichtigung gesendet.)

Weitere [ausführliche Informationen zu den Benachrichtigungen die](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) sind verfügbar.

**Verwalten von Benachrichtigungen**

Benutzer müssen ihre eigenen Benachrichtigungen verwalten. Informationen hierzu finden Sie unter [Aktivieren und Deaktivieren von Yammer-E-Mails und mobilen Benachrichtigungen](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratoren können nicht alle Benachrichtigungen für die Benutzer deaktivieren oder Benachrichtigungen in deren Namen steuern. Administratoren können [das in E-Mails enthaltene Logo steuern und festlegen, ob Benutzer Nachrichten bestätigen müssen](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer), die per E-Mail gepostet werden.

**An viele Benutzer in Ihrer Organisation gesendete E-Mail-Benachrichtigungen**

Es kann vorkommen, dass eine einzige E-Mail-Benachrichtigung von Yammer gesendet und von viel mehr Benutzern in Ihrer Organisation empfangen wird, als erwartet. Dies geschieht, wenn eine Verteilerliste oder eine andere Art von E-Mail-Adresse, die keiner Einzelperson zugeordnet ist, zu Yammer hinzugefügt wird. Yammer erkennt nicht in allen Fällen, ob eine E-Mail-Adresse zu einem einzelnen Benutzer gehört oder eine E-Mail-Adresse ist, die bewirkt, dass eine E-Mail-Nachricht an viele Empfänger übermittelt wird. Wenn dieses Problem auftritt, müssen Sie Maßnahmen ergreifen, um den [ungültigen Benutzer mit dieser E-Mail-Adresse in Yammer zu sperren (deaktivieren)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users). 

Um die Wahrscheinlichkeit zu verringern, dass dieses Problem auftritt, sollten Sie Folgendes tun:

1. [Erzwingen der Office 365-Identität](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) für Yammer.
2. Sperren externer Absendern, um das Senden von E-Mails an Ihre Organisation zu verhindern, oder Beschränken der Absender auf eine Liste genehmigter Absender.

Wenn dieses Problem auftritt:

1. Ermitteln Sie den E-Mail-Empfänger, der dem Benutzer in Yammer entsprechen soll. Beispielsweise ist "all-in-Sales@fabrikam.com" eine Verteilerliste für alle Vertriebsmitarbeiter. Diese Verteilerliste wäre anhand der von Benutzern empfangenen Yammer-E-Mails identifizierbar.
2. Verwenden Sie das [Feature "Deaktivieren" (Sperren) unter "Netzwerkadministrator"](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users), um den Benutzer mit der E-Mail-Adresse "all-in-Sales@fabrikam.com" zu sperren. Die Sperrung kann rückgängig gemacht werden, daher ist Sie sicherer als das Löschen. Das Löschen des Benutzers erfolgt automatisch nach 90 Tagen.
3. Überprüfen Sie optional den [Export der Benutzer](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), um andere nicht von Benutzern stammenden E-Mail-Adressen zu identifizieren, die gesperrt werden sollten.
