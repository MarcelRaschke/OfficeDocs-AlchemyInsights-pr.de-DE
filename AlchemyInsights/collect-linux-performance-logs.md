---
title: Sammeln von Linux-Leistungsprotokollen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010721"
- "17373"
ms.openlocfilehash: 25a711a09e1a79837a4a714d7c723fb9f4f3707a
ms.sourcegitcommit: 9edb4aa99886a74c1f391d1927d5f8d16d6b6904
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65552005"
---
# <a name="collect-linux-performance-logs"></a>Sammeln von Linux-Leistungsprotokollen

**Ausführen der Analyse über das GUI-Szenario**

1. Laden Sie das [XMDE Client Analyzer-Tool](https://aka.ms/XMDEClientAnalyzer) auf den macOS oder Linux-Computer herunter, den Sie untersuchen müssen.

    **Hinweis** Der aktuelle SHA256-Hash von "XMDEClientAnalyzer.zip", der vom obigen Link heruntergeladen wurde, lautet:

    "A9BF065DE3F2608A309BC4F5295548BB9931F107BF2F01DC42A789C5527C1308".
1. Extrahieren Sie den Inhalt von XMDEClientAnalyzer.zip auf dem Computer.
1. Öffnen Sie eine Terminalsitzung, ändern Sie das Verzeichnis in den extrahierten Speicherort, und führen Sie Folgendes aus:

    `./mde_support_tool.sh -d`

**Hinweis** Wenn das Skript unter Linux nicht zum Ausführen berechtigt ist, müssen Sie zuerst Folgendes ausführen:

`chmod a+x mde_support_tool.sh`

**Ausführen des Analyzers mithilfe eines Terminal- oder SSH-Szenarios**

Öffnen Sie ein Terminal oder SSH auf dem entsprechenden Computer, und führen Sie die folgenden Befehle aus:

1. Laden Sie das [XMDE Client Analyzer-Tool](https://aka.ms/XMDEClientAnalyzer) auf den macOS oder Linux-Computer herunter, den Sie untersuchen und ausführen müssen:

    wget --quiet -O XMDEClientAnalyzer.zip

1. Entzippen Sie -q XMDEClientAnalyzer.zip
1. cd XMDEClientAnalyzer
1. chmod +x mde_support_tool.sh
1. Ausführen als Nicht-Stammanwendung zum Installieren der erforderlichen Pip- und lxml-Komponenten: ./mde_support_tool.sh
1. Um das eigentliche Diagnosepaket zu sammeln und die Ergebnisarchivdatei zu generieren, führen Sie die Datei erneut als Stammdatei aus: ./mde_support_tool.sh -d

**Notizen** 

- Für Linux erfordert die Analyse lxml, um die Ergebnisausgabe zu erzeugen. Wenn lxml nicht installiert ist, versucht der Analyzer, es aus dem offiziellen Repository für die folgenden Python-Pakete abzurufen: `https://files.pythonhosted.org/packages/\*/lxml\*.whl`

- Das Tool erfordert Python Version 3 oder höher. Wenn Sie auf einem Computer ausgeführt werden, der Python 3 nicht verwenden oder die lxml-Komponente abrufen kann, können Sie [XMDE Client Analyzer Binary](https://aka.ms/XMDEClientAnalyzerBinary) herunterladen.

- Wenn sich Ihr Gerät hinter einem Proxy befindet, können Sie den Proxyserver einfach als Umgebungsvariable an das skript mde_support_tool.sh übergeben. Beispiel: `https_proxy=https://myproxy.contoso.com:8080 ./mde_support_tool.sh"`

Hilfe zur Befehlszeilensyntax:

-h # Hilfe

Zeigt die Hilfenachricht an.

Leistung # Leistung

Sammelt eine umfassende Ablaufverfolgung für die Analyse eines Leistungsproblems, das bei Bedarf reproduziert werden kann. Verwenden von --length=*seconds* zum Angeben der Dauer des Benchmarks.

-o # Ausgabe

Gibt den Zielpfad für die Ergebnisdatei an.

-nz # No-Zip

Wenn festgelegt, wird ein Verzeichnis anstelle einer resultierenden Archivdatei erstellt.

-f # Force

Erzwingen Sie das Überschreiben, wenn die Ausgabe bereits am Zielpfad vorhanden ist.

**Ergebnispaketinhalte unter macOS und Linux**

- report.html Beschreibung: Die html-Ausgabedatei, die die Ergebnisse und Anleitungen enthält, die das auf dem Computer ausgeführte Analyseskript erzeugen kann.
- mde_diagnostic.zip Beschreibung: Dieselbe Diagnoseausgabe, die beim Ausführen der Mdatp-Diagnose generiert wird, die entweder unter macOS oder Linux erstellt wurde.
- mde.xml Beschreibung: Während der Ausführung generierte XML-Ausgabe und wird zum Erstellen der HTML-Berichtsdatei verwendet.
- Processes_information.txt Beschreibung: Enthält die Details der ausgeführten Microsoft Defender für Endpunkt zugehörigen Prozesse auf dem System.
- Log.txt Beschreibung: Enthält dieselben Protokollmeldungen, die während der Datensammlung auf dem Bildschirm geschrieben wurden.
- Health.txt Beschreibung: Die gleiche grundlegende Integritätsausgabe, die beim Ausführen des mdatp-Integritätsbefehls angezeigt wird.
- Events.xml Beschreibung: Zusätzliche XML-Datei, die vom Analysetool beim Erstellen des HTML-Berichts verwendet wird.
- Auditd_info.txt Beschreibung: Details zu überwachten Diensten und zugehörigen Komponenten für Linux-Betriebssystem.
- perf_benchmark.tar.gz Beschreibung: Die Leistungstestberichte werden nur angezeigt, wenn Sie den Leistungsparameter verwenden.
