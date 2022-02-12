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
ms.openlocfilehash: ceb714ec80f346f6e71ce966b45159271668af8e
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62722077"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Doppelklicken auf eine Office Datei kann nicht geöffnet werden

Nachdem Sie auf eine Office Datei geklickt haben, wird das Programm möglicherweise geöffnet, die Datei selbst wird jedoch nicht geöffnet. Oder Sie erhalten die Fehlermeldung: "Beim Senden des Befehls an das Programm ist ein Problem aufgetreten." Dafür gibt es viele Ursachen, aber die beiden gängigsten Lösungen sind:

- Stellen Sie in Excel sicher, dass die DDE-Option deaktiviert ist. Die Option finden Sie, indem Sie eine neue Arbeitsmappe erstellen und dann **Datei > Optionen > Erweitert** auswählen. Deaktivieren Sie im Abschnitt **"Allgemein**" die Option **"Andere Anwendungen ignorieren", die dynamische Daten Exchange (DDE) verwenden**.

- Führen Sie eine Onlinereparatur aus, um die Standardeinstellungen wiederherzustellen. Klicken Sie auf die schaltfläche Windows Start, und suchen Sie nach "Systemsteuerung". Öffnen **Sie die Systemsteuerung**, und wechseln Sie zu **"Programme > Programme und Features"**. Klicken Sie dann mit der rechten Maustaste auf **Microsoft Office [Version],** und wählen Sie **"> Onlinereparatur ändern**" aus.

Wenn keine dieser Lösungen funktioniert, finden Sie im Supportartikel eine vollständigere Liste von Lösungen. [Wenn Sie auf eine Office Datei doppelklicken, wird sie nicht geöffnet](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
