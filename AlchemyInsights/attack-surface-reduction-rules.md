---
title: Regeln zur Verringerung der Angriffsfläche
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: da2c9b3b1c729ab2fe4c4388287d56a4f7c39912
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61864228"
---
# <a name="attack-surface-reduction-rules"></a>Regeln zur Verringerung der Angriffsfläche

Das Ausschließen von Dateien oder Ordnern kann den Schutz durch Regeln zur Verringerung der Angriffsfläche erheblich beeinträchtigen. Dateien, die durch eine Regel blockiert worden wären, dürfen ausgeführt werden, und es wird kein Bericht oder Ereignis aufgezeichnet. Ein Ausschluss gilt für alle Regeln, die Ausschlüsse zulassen.

ASR-Ausschlüsse verwenden dieselbe Syntax wie Microsoft Defender Antivirus-Ausschlüsse. Weitere Informationen finden Sie unter [Konfigurieren und Überprüfen von Ausschlüssen für Microsoft Defender Antivirus-Scans](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Um Probleme zu vermeiden, lesen Sie [Häufige Fehler, die beim Festlegen von Ausschlüssen vermieden werden sollten](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Nicht alle ASR-Regeln unterstützen Ausschlüsse. Informationen zur Überprüfung, ob Ihre Regel Ausschlüsse unterstützt, finden Sie in der Tabelle [Regeln zur Verringerung der Angriffsfläche](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regeln zur Verringerung der Angriffsfläche

Die Angriffsfläche Ihrer Organisation enthält alle Stellen, an denen ein Angreifer Geräte oder Netzwerke der Organisation gefährden könnte. Die Verringerung ihrer Angriffsoberfläche bedeutet, die Geräte und das Netzwerk des Unternehmens zu schützen, sodass Angreifer weniger Möglichkeiten haben, Angriffe auszuführen. Das Konfigurieren von Regeln zur Verringerung der Angriffsfläche in Microsoft Defender für Endpunkt kann dabei hilfreich sein.

Weitere Informationen finden Sie unter:

- [Zuordnen des ASR-Regel-GUID zu Namen](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Voraussetzungen der ASR-Regeln:
    - [Windows 10, Version 1709 oder höher](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, Version 1709 oder höher](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, Version 1803 (halbjährlicher Kanal) oder höher](https://docs.microsoft.com/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifizieren Sie den richtigen, anzuwendenden Ausschluss.

1. Suchen Sie im Microsoft-Windows-Windows Defender/ Betriebsprotokoll nach eventID 1121 oder 1122.

1. Werten Sie das Blockierungsszenario und den Kontext aus und bestätigen Sie, dass dieses Szenario entsperrt werden soll.

1. Lesen Sie den Pfadwert in den Ereignisdetails. Dies ist der Wert, der den Ausschluss definiert.
    - Machen Sie den Ausschluss so streng wie möglich.
    - Wenden Sie bei Bedarf einen Platzhalter an (ersetzen Sie beispielsweise die Benutzervariable).

1. Wenden Sie den Ausschluss entsprechend Ihren Bereitstellungsanforderungen an. Weitere Informationen finden Sie unter [Anpassen der Regeln zur Verringerung der Angriffsfläche](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Ausschluss wird nicht anerkannt

1. Bestimmen Sie, ob die Regel Ausschlüsse unterstützt. Weitere Informationen finden Sie unter [Anpassen der Regeln zur Verringerung der Angriffsfläche](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Überprüfen Sie die angewendeten Ausschlüsse und überprüfen Sie anhand der Ereignisdaten, ob Tippfehler oder falsch interpretierte Platzhalter vorhanden sind. Weitere Informationen finden Sie unter [Unterstützte Ausschlusstypen](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Wenn die Auswirkung der Regel zu hoch ist, sollten Sie die Regel (zurück) in den Überwachungsmodus verschieben, um eine weitere Validierung durchzuführen. Weitere Informationen finden Sie unter [Testen der Funktionalität der Features von Microsoft Defender für Endpunkte im Überwachungsmodus](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Sammeln Sie Supportdaten, um einen Supportfall mit diesem Befehl zu öffnen:
    
   ** MDEClientAnalyzer.cmd -v**
