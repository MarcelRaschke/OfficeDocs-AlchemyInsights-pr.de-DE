---
title: Ausführen von Windows-Speicherdiagnose in Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: df9a717700f4cf94104b666554c85d6080d6bd4f
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61945222"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Ausführen von Windows-Speicherdiagnose in Windows 10

Wenn Windows und Apps auf Ihrem PC abstürzen, einfrieren oder sich instabil verhalten, haben Sie möglicherweise ein Problem mit dem Arbeitsspeicher (RAM) des PCs. Sie können die Windows-Speicherdiagnose ausführen, um nach Problemen mit dem Arbeitsspeicher des PCs zu suchen.

Geben Sie in das Suchfeld in der Taskleiste **Speicherdiagnose** ein, und wählen Sie dann **Windows-Speicherdiagnose**. 

Um die Diagnose auszuführen, muss der PC neu gestartet werden. Sie haben die Möglichkeit, sofort neu zu starten (bitte speichern Sie Ihre Arbeit und schließen Sie zuerst geöffnete Dokumente und E-Mails), oder Sie können die Diagnose so planen, dass sie beim nächsten Neustart des PCs automatisch ausgeführt wird:

![Windows-Speicherdiagnose](media/windows-memory-diagnostic.png)

Wenn der PC neu gestartet wird, wird das **Windows-Speicherdiagnosetool** automatisch ausgeführt. Status und Fortschritt werden während des Diagnoselaufs angezeigt, und Sie haben die Möglichkeit, die Diagnose durch Drücken der Taste **ESC** auf Ihrer Tastatur abzubrechen.

Nach Abschluss der Diagnose wird Windows normal gestartet.
Unmittelbar nach dem Neustart, wenn der Desktop angezeigt wird, erscheint eine Benachrichtigung (neben dem Symbol  **Info-Center** in der Taskleiste), um anzuzeigen, ob Speicherfehler gefunden wurden. Zum Beispiel:

Das ist das Symbol „Info-Center“: ![Symbol „Info-Center“](media/action-center-icon.png) 

Und eine Beispiel-Benachrichtigung: ![Keine Speicherfehler](media/no-memory-errors.png)

Wenn Sie die Benachrichtigung verpasst haben, können Sie das Symbol **Info-Center** in der Taskleiste wählen, um das **Info-Center** anzuzeigen und eine scrollbare Liste der Benachrichtigungen zu sehen.

Um detaillierte Informationen zu überprüfen, geben Sie das **Ereignis** in das Suchfeld in Ihrer Taskleiste ein und wählen Sie dann **Ereignisanzeige**. Navigieren Sie im linken Fensterbereich der **Ereignisanzeige** zu **Windows-Protokolle > System**. Scannen Sie im rechten Fensterbereich die Liste nach unten, während Sie die Spalte **Quelle** betrachten, bis Sie Ereignisse mit dem Quellenwert **MemoryDiagnostics-Results** sehen. Markieren Sie jedes dieser Ereignisse und sehen Sie die Ergebnisinformationen im Feld unter der Registerkarte **Allgemein** unterhalb der Liste.
