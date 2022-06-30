---
title: 'Häufig gestellte Fragen zur Nachrichtenablaufverfolgung in Exchange Online '
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010086"
- "15388"
ms.openlocfilehash: c1ff8f2b03f97e7465a44a983670530055d19889
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66411889"
---
# <a name="frequently-asked-questions-for-message-trace-in-exchange-online"></a>Häufig gestellte Fragen zur Nachrichtenablaufverfolgung in Exchange Online

Als Administrator können Sie herausfinden, was mit einer E-Mail passiert ist, indem Sie eine Nachrichtenablaufverfolgung im Exchange-Verwaltungskonsole (EAC) ausführen. Es folgen einige der häufig gestellten Fragen zur Nachrichtenablaufverfolgung in Exchange Online:

**Ich benötige den Status der gesendeten Nachrichten, die älter als 90 Tage sind. Gibt es eine andere Möglichkeit, den Status von Nachrichten zu sammeln?**

Standardmäßig ruft Exchange Online Nachrichtenablaufverfolgung Daten aus den letzten 90 Tagen ab. Wenn Sie Nachrichtenablaufverfolgungsdaten benötigen, die älter als 90 Tage sind, können Sie ein Skript erstellen, um die Daten in regelmäßigen Abständen von Microsoft 365 abzurufen und mithilfe des cmdlets Get-MessageTrace im lokalen Repository zu speichern. Alternativ können Sie eine Inhaltssuche nach E-Mails durchführen, die älter als 90 Tage sind. Weitere Informationen finden [Sie unter Erstellen und Ausführen einer Inhaltssuche im Microsoft Purview-Complianceportal](https://docs.microsoft.com/microsoft-365/compliance/content-search).

**Was ist die Zeitzone, die auf der Nachrichtenverfolgungsschnittstelle angezeigt wird?**

Die Benutzeroberfläche der Nachrichtenablaufverfolgung zeigt die Uhrzeit entsprechend der lokalen Zeitzone an. Wenn ein Administrator jedoch Ergebnisse in eine CSV-Datei exportiert, zeigt die exportierte Datei das Datum/die Uhrzeit in UTC an.

**Gewusst wie Nachrichtenablaufverfolgungsergebnisse in eine CSV-Datei exportieren?**

Die Ergebnisse der Nachrichtenablaufverfolgung können exportiert werden, indem Sie in der oberen linken Ecke der Suchergebnisse der Nachrichtenablaufverfolgung die Schaltfläche " **Ergebnisse exportieren** " auswählen. Alternativ können Sie den [PowerShell-Befehl "Get-MessageTrace](https://docs.microsoft.com/powershell/module/exchange/get-messagetrace)" ausführen. Hier ist ein Beispiel:

```Get-MessageTrace -SenderAddress "Email address of the sender" -StartDate 06/13/2012 -EndDate 06/15/2012 | FL > D:\report.csv```

Sie können auch Start-HistoricalSearch ausführen, um weitere Informationen zu einer bestimmten Nachricht zu exportieren und anzuzeigen. Ausführliche Informationen finden [Sie unter Start-HistoricalSearch](https://docs.microsoft.com/powershell/module/exchange/start-historicalsearch).

**Was bedeutet der Zustellungsstatus für die Nachrichtenablaufverfolgungsausgabe?**

- **Zugestellt**: Die Nachricht wurde erfolgreich an das beabsichtigte Ziel übermittelt.
- **Fehler**: Die Nachricht wurde nicht zugestellt. Entweder wurde die Zustellung versucht und ist fehlgeschlagen, oder die Nachricht wurde aufgrund von Aktionen des Filterdiensts nicht übermittelt. Dies ist beispielsweise der Fall, wenn die Nachricht angeblich Schadsoftware enthält.
- **Ausstehend**: Die Zustellung der Nachricht wird versucht oder erneut versucht.
- **Erweitert**: Die Nachricht wurde an eine Verteilerliste gesendet und erweitert, sodass die Mitglieder der Liste einzeln angezeigt werden können.
- **Als Spam gefiltert**: Die Nachricht wurde an den Junk-E-Mail-Ordner übermittelt.
- **Unbekannt**: Der Nachrichtenübermittlungsstatus ist zurzeit unbekannt. Wenn die Ergebnisse der Abfrage aufgelistet werden, enthält das Feld "Übermittlungsdetails" keine Informationen.

Weitere Informationen finden Sie unter [Ausführen einer Nachrichtenablaufverfolgung im klassischen EAC in Exchange Online](https://docs.microsoft.com/exchange/monitoring/trace-an-email-message/run-a-message-trace-and-view-results).
