---
title: Doppelklicken auf eine Office Datei kann nicht geöffnet werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 847aa465633ca2d37deb8dabd332e509e8b85fec
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61972581"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Doppelklicken auf eine Office Datei kann nicht geöffnet werden

Nachdem Sie auf eine Office Datei geklickt haben, wird möglicherweise das Programm geöffnet, die Datei selbst wird jedoch nicht geöffnet. Oder Sie erhalten die Fehlermeldung: "Beim Senden des Befehls an das Programm ist ein Problem aufgetreten." Dafür gibt es viele Ursachen, aber die beiden gängigsten Lösungen sind:

- Stellen Sie in Excel sicher, dass die DDE-Option deaktiviert ist. Die Option finden Sie, indem Sie eine neue Arbeitsmappe erstellen und dann **Datei > Optionen > Erweitert** auswählen. Deaktivieren Sie im Abschnitt **"Allgemein"** die Option **"Andere Anwendungen ignorieren", die dynamic Data Exchange (DDE) verwenden.**

- Führen Sie eine Onlinereparatur aus, um die Standardeinstellungen wiederherzustellen. Klicken Sie auf die Windows Startschaltfläche, und suchen Sie nach "Systemsteuerung". Öffnen Sie die **Systemsteuerung,** und wechseln Sie zu **"Programme > Programme und Features".** Klicken Sie dann mit der rechten Maustaste auf **Microsoft Office [Version],** und wählen Sie **"> Onlinereparatur ändern"** aus.

Wenn keine dieser Lösungen funktioniert, finden Sie im Supportartikel eine vollständigere Liste von Lösungen. [Wenn Sie auf eine Office Datei doppelklicken,](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)wird sie nicht geöffnet.
