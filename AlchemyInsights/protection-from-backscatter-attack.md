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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 74715db1f8177cb6229f21a6155400bdcaa337bf
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63252994"
---
# <a name="protection-from-backscatter-attack"></a>Schutz vor Backscatter-Angriffen

Backscatter sind Nichtzustellungsberichte (auch als NDRs oder Bounce-Nachrichten bezeichnet), die Sie für Nachrichten erhalten, die Sie nicht gesendet haben. Spammer fälschen (spoofen) die **Absender**-Adresse ihrer Nachrichten und verwenden häufig echte E-Mail-Adressen, um ihren Nachrichten Glaubwürdigkeit zu verleihen. Wenn Spammer unweigerlich Nachrichten an nicht vorhandene Empfänger senden, wird der Ziel-E-Mail-Server im Wesentlichen dazu verleitet, die nicht zustellbare Nachricht in einem NDR an den gefälschten Absender in der **Absender:**-Adresse zurückzugeben.

Weitere Informationen finden Sie in [Backscatter in Exchange Online Protection (EOP)](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

Sie müssen den Backscatter-Schutz in Antispamrichtlinien in den folgenden Umgebungen nicht aktivieren, da legitime Unzustellbarkeitsberichte übermittelt und Backscatter als Spam gekennzeichnet werden:

- Organisationen mit Exchange Online Postfächern.
- Lokale E-Mail-Organisationen, in denen **ausgehende** E-Mails über EOP weitergeleitet werden.

In eigenständigen EOP-Organisationen, die **eingehende** E-Mails an lokale Postfächer schützen, ermöglicht das Aktivieren des Backscatter-Schutzes in Antispamrichtlinien die Zustellung legitimer Unzustellbarkeitsberichte und die Markierung von Backscatter als Spam.

Führen Sie die folgenden Schritte aus, um den Backscatter-Schutz in Antispamrichtlinien zu aktivieren:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail und Zusammenarbeit** \> **Richtlinien und Regeln** \> **Bedrohungsrichtlinien** \> **Antispam** im Abschnitt **Richtlinien**.

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **Antispamrichtlinien** die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken (**Type** ist **Benutzerdefinierte Antispamrichtlinie** oder **Name** ist **Antispam-Eingangsrichtlinie (Standard)**).

3. Klicken Sie im angezeigten Detailflyout auf **Spamschwellenwert und Eigenschaften bearbeiten** im Abschnitt **Schwellenwert für Massen-E-Mails und Spam-Eigenschaften**.

4. Suchen Sie im Abschnitt **Als Spam markieren** die Option **Backscatter**, und wählen Sie den Wert **Ein** aus.

Wenn Sie der Meinung sind, dass ein Konto kompromittiert wurde, lesen Sie Folgendes:

- [Auf ein kompromittiertes E-Mail-Konto reagieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Entfernen blockierter Benutzer aus dem Portal für eingeschränkte Benutzer](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)
