---
title: MsMpEng.exe verbraucht übermäßige CPU
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010633"
- "17605"
ms.openlocfilehash: a76237a9449578bd1a6ee3c2cb0e03572ee80e40
ms.sourcegitcommit: 6bb8dd2dc45a4efe2469c9db430cd36fdb6a7fea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66504240"
---
# <a name="msmpengexe-is-consuming-excessive-cpu"></a>MsMpEng.exe verbraucht übermäßige CPU

1. Laden Sie den [Datensammler der Microsoft Defender für Endpunkt (MDE)-Clientanalyse](https://aka.ms/Betamdeanalyzer) herunter.

1. Extrahieren Sie das Paket in ein Verzeichnis auf dem Computer mit der hohen CPU-Auslastung innerhalb MsMpEng.exe.

1. Öffnen Sie eine Eingabeaufforderung.

1. Wechseln Sie im Administrativen Eingabeaufforderungsfenster zum Verzeichnis der extrahierten Clientanalyse. Beispiel:

    cd "C:\temp\MDEClientAnalyzerPreview"

1. Ausführen des Befehls: MDEClientAnalyzer -a -v

1. Nach einigen grundlegenden Überprüfungen werden Sie aufgefordert, den Zeitraum für die Ausführung der Ablaufverfolgung festzulegen. Geben Sie eine Zeit in Minuten ein; bei hoher CPU-Auslastung beträgt die empfohlene Zeit 1-5 Minuten.

    Client Analyzer-Text: **Geben Sie die Anzahl der Minuten ein, um Ablaufverfolgungen zu sammeln:**

1. Nach Abschluss der Datensammlung befindet sich ein komprimiertes Paket in dem Ordner, aus dem Sie die Clientanalyse ausgeführt haben. Beispiel:

    C:\temp\MDEClientAnalyzerPreview\MDEClientAnalyzerResult.zip

1. Fügen Sie dieses Datenpaket an Ihren Supportfall an.