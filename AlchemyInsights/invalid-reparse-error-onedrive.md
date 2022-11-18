---
title: Fehler eines ungültigen Analysepunktpuffers in OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9011272"
- "18277"
ms.openlocfilehash: 4e2ce46ec9d99242397cea0357f4603a2fb70960
ms.sourcegitcommit: ac762f4ee4f63cb732e2090f0d152fb2368421bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/12/2022
ms.locfileid: "67646979"
---
# <a name="invalid-reparse-point-buffer-error-in-onedrive"></a>Fehler eines ungültigen Analysepunktpuffers in OneDrive

Wenn Sie versuchen, eine Datei aus dem lokalen synchronisierten Ordner zu löschen, wird möglicherweise die Fehlermeldung "Die im Analysepunktpuffer vorhandenen Daten sind ungültig" angezeigt.

Wenn der Analysepunkt ungültig `ChkDsk` ist und `fsutil` in der Regel entfernt werden kann:

1. Öffnen Sie eine Administrator-Eingabeaufforderung, indem Sie " **Start**" auswählen, **nach "cmd**" suchen und dann " **Als Administrator ausführen**" auswählen.
1. Führen Sie den Folgenden Befehl aus: `chkdsk c: /R /F`
1. Die Meldung "Chkdsk kann nicht ausgeführt werden, weil das Volume von einem anderen Prozess verwendet wird" wird angezeigt. Möchten Sie planen, dass dieses Volume beim nächsten Neustart des Systems überprüft wird? (Y/N)."
1. Geben Sie **Y ein,** und drücken **Sie die EINGABETASTE**.
1. Starten Sie den Computer neu, um den Computer auszuführen `Chkdsk`.