---
title: Senden einer E-Mail-Nachricht durch Angeben der Netzwerknachrichten-ID
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c0450324b0f2903382f463797b8e41f80066fcd
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66393231"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Senden einer E-Mail-Nachricht durch Angeben der Netzwerknachrichten-ID

1. Wählen Sie im Flyout " **Neue Übermittlung** " **die Option "E-Mail-** und **Netzwerknachrichten-ID**" aus.
2. Führen Sie die folgenden Schritte aus, um die Nachrichten-ID für eine E-Mail-Nachricht in Outlook zu finden:
    1. Doppelklicken Sie auf die E-Mail-Nachricht, um sie zu öffnen.
    1. Wählen Sie **"Dateieigenschaften** > **" aus**.
    1. Öffnen Sie Editor oder ein leeres Word-Dokument, und kopieren Sie dann den Inhalt, der sich im **Feld "Internetkopfzeilen** " befindet, und fügen Sie ihn in das geöffnete Dokument ein, um die Sichtbarkeit zu verbessern.
    1. Suchen Sie das Feld **"X-MS-Exchange-Organization-Network-Message-ID** ". Der Wert nach dem **:** ist die ID, die Sie für Ihre Übermittlung benötigen.
3. Wenn die E-Mail unter **"Empfänger**" für alle Empfänger dieser E-Mail im Junk-E-Mail-Ordner landete, wählen **Sie "Alle auswählen"** aus. Wenn nicht, wählen Sie nur den Benutzer aus, der das Problem gemeldet hat.
4. Wenn Sie unter **"Grund für die Übermittlung**" die Option **"Hätte blockiert"** auswählen, geben Sie an, ob die Nachricht als **Spam**, **Phishing** oder **Schadsoftware** blockiert worden sein soll, und wählen Sie dann **"Absenden**" aus.

Weitere Informationen finden Sie unter [So senden Sie verdächtigen Spam, Phishing, URLs und Dateien zur Überprüfung an Microsoft](https://go.microsoft.com/fwlink/?linkid=2101479).
