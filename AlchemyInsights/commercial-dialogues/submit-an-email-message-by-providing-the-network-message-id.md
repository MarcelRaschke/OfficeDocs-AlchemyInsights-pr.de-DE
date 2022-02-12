---
title: Senden einer E-Mail-Nachricht durch Angeben der Netzwerknachrichten-ID
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c70655584a5162afaf75945a0728c412d1cf52fa
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62687480"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Senden einer E-Mail-Nachricht durch Angeben der Netzwerknachrichten-ID

1. Wählen Sie im Flyout **"Neue Übermittlung** " die **E-Mail-** und **Netzwerknachrichten-ID** aus.
2. Führen Sie die folgenden Schritte aus, um die Nachrichten-ID für eine E-Mail-Nachricht in Outlook zu finden:
    1. Doppelklicken Sie auf die E-Mail-Nachricht, um sie zu öffnen.
    1. Wählen Sie **"****FileProperties** > " aus.
    1. Öffnen Sie Editor oder ein leeres Word-Dokument, und kopieren Sie dann den Inhalt im **Internetkopfzeilenfeld**, und fügen Sie ihn in das geöffnete Dokument ein, um eine bessere Sichtbarkeit zu gewährleisten.
    1. Suchen Sie das **Feld "X-MS-Exchange-Organization-Network-Message-Id**". Der Wert nach dem **:** ist die ID, die Sie für Ihre Übermittlung benötigen.
3. Wenn die E-Mail für alle Empfänger dieser E-Mail im Junk-E-Mail-Ordner gelandet ist, wählen Sie unter " **Empfänger**" die Option **"Alle auswählen**" aus. Wenn nicht, wählen Sie nur den Benutzer aus, der das Problem gemeldet hat.
4. Geben Sie unter **dem Grund für die Übermittlung**, wenn Sie **"Sollte blockiert" ausgewählt haben**, an, ob die Nachricht als **Spam**, **Phishing** oder **Schadsoftware** blockiert worden sein soll, und wählen Sie dann " **Übermitteln**" aus.

Weitere Informationen finden Sie unter ["Übermitteln von verdächtigem Spam, Phishing, URLs und Dateien zur Überprüfung an Microsoft](https://go.microsoft.com/fwlink/?linkid=2101479)".
