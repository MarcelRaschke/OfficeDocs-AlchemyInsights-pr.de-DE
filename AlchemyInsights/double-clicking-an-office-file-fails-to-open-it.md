---
title: Durch Doppelklicken auf eine Office-Datei kann sie nicht geöffnet werden.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 12a8d137781b3a708a542e4f13c9a92ad190142a
ms.sourcegitcommit: 8324c868c664bfdee6d5bb99ad8d41e9dd46d10f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66537722"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Durch Doppelklicken auf eine Office-Datei kann sie nicht geöffnet werden.

Nach dem Doppelklicken auf eine Office-Datei wird das Programm möglicherweise geöffnet, aber die Datei selbst wird nicht geöffnet. Oder Sie erhalten die Fehlermeldung: "Problem beim Senden des Befehls an das Programm." Dafür gibt es viele Ursachen, aber die beiden am häufigsten verwendeten Lösungen sind:

- Stellen Sie in Excel sicher, dass die DDE-Option deaktiviert ist. Die Option finden Sie, indem Sie eine neue Arbeitsmappe erstellen und dann **"Datei > Optionen" > "Erweitert**" auswählen. Deaktivieren Sie im Abschnitt **"Allgemein** " das Kontrollkästchen **"Andere Anwendungen ignorieren", die dynamischen Datenaustausch (Dynamic Data Exchange, DDE) verwenden**.

- Führen Sie eine Onlinereparatur aus, um die Standardeinstellungen wiederherzustellen. Klicken Sie auf die Windows-Schaltfläche "Start", und suchen Sie nach "Systemsteuerung". Öffnen Sie die **Systemsteuerung**, und wechseln Sie zu **"Programme > Programme und Features"**. Klicken Sie dann mit der rechten Maustaste auf **Microsoft Office [Version],** und wählen **Sie "> Onlinereparatur ändern**" aus.

Wenn keine dieser Lösungen funktioniert, finden Sie eine vollständigere Liste der Lösungen im Supportartikel. Wenn [Sie auf eine Office-Datei doppelklicken, wird sie nicht geöffnet](https://support.microsoft.com/office/double-clicking-an-office-file-fails-to-open-it-in-the-correct-office-program-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
