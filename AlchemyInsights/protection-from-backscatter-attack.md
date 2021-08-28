---
title: Schutz vor Backscatter-Angriffen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8c6b1cfe79d322702279877ff351397a366fa246710c04e25181a675ad2fdeab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911229"
---
# <a name="protection-from-backscatter-attack"></a>Schutz vor Backscatter-Angriffen

Backscatter sind Nichtzustellungsberichte (auch als NDRs oder Bounce-Nachrichten bezeichnet), die Sie für Nachrichten erhalten, die Sie nicht gesendet haben. Spammer fälschen (spoofen) die **Absender**-Adresse ihrer Nachrichten und verwenden häufig echte E-Mail-Adressen, um ihren Nachrichten Glaubwürdigkeit zu verleihen. Wenn Spammer unweigerlich Nachrichten an nicht vorhandene Empfänger senden, wird der Ziel-E-Mail-Server im Wesentlichen dazu verleitet, die nicht zustellbare Nachricht in einem NDR an den gefälschten Absender in der **Absender:**-Adresse zurückzugeben.

Weitere Informationen finden Sie in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Aktivieren des Backscatter-Schutzes**

Folgen Sie dem folgenden Pfad, um den Backscatter-Schutz zu aktivieren.

**protected.office.com > Bedrohungsmanagement > Richtlinie > Antispam > Wählen Sie die Spamfilterrichtlinie aus und bearbeiten Sie die Richtlinie > Spam-Eigenschaften > Als Spam markieren > NDR-Backscatter > Schalten Sie diese auf "Ein"**.

Wenn Sie der Meinung sind, dass ein Konto kompromittiert wurde, lesen Sie Folgendes:

- [Auf ein kompromittiertes E-Mail-Konto reagieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Entfernen blockierter Benutzer aus dem Portal "Eingeschränkte Benutzer" in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



