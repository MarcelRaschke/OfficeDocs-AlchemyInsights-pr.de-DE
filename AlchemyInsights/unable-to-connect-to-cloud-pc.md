---
title: Verbindung zum Cloud-PC kann nicht hergestellt werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9008608"
- "14008"
ms.openlocfilehash: f84c398f5d1f31012816f82f7866059f76c3c2d7
ms.sourcegitcommit: b52a81c62e8ec915617cf4939abf271139b87f69
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2022
ms.locfileid: "67883204"
---
# <a name="unable-to-connect-to-cloud-pc"></a>Verbindung zum Cloud-PC kann nicht hergestellt werden

Es gibt mehrere mögliche Ursachen dafür, dass keine Verbindung mit einem Cloud-PC hergestellt werden kann. Der Großteil der aufgetretenen Probleme bezieht sich direkt auf Probleme mit der Netzwerkkonnektivität an einer beliebigen Stelle im Netzwerkpfad zwischen dem Client-PC, der für die Verbindung verwendet wird, und dem Cloud-PC. Es ist auch möglich, dass Einstellungen auf dem Client-PC und dem Cloud-PC das Netzwerkverhalten beeinflussen.

Für Windows 365 Enterprise Kunden ist die Konnektivität zwischen dem Cloud-PC und den lokalen Domänencontrollern auch ein potenzieller Pfad für Netzwerkprobleme.

Für Windows 365 Enterprise Kunden kann die Anwendung von Netzwerk- und Richtlinieneinstellungen, die auf Ihre lokalen Windows-PCs angewendet werden, die Konnektivität von Windows 365 Cloud-PCs beeinträchtigen. Ein nützlicher Schritt zur Problembehandlung kann darin sein, die betroffenen Cloud-PCs in eine separate OE zu verschieben, die vom Empfang Gruppenrichtlinie blockiert wird, um die von GPO bereitgestellte Einstellung als zugrunde liegenden Konnektivitätsblocker zu beseitigen.

Hier sind beispiele für häufige Fehlermeldungen und deren ursachen:

**Fehler**: "Wir konnten keine Verbindung herstellen, weil derzeit keine Ressourcen verfügbar sind."

**Ursachen**: Der Cloud-PC, mit dem Sie eine Verbindung herstellen möchten, hat die Bereitstellung nicht abgeschlossen. Die Bereitstellungszeit ist variabel und kann 45 Minuten überschreiten.

**Fehler**: "Wir konnten aufgrund eines Fehlers keine Verbindung mit dem Gateway herstellen. Wenn dies weiterhin geschieht, bitten Sie Ihren Administrator oder technischen Support um Hilfe."

**Ursachen**: Netzwerkkonfigurationsprobleme können Folgendes umfassen, sind aber nicht beschränkt auf:

- Benutzerdefinierte DNS-Einstellungen 
- Blockade des virtuellen Netzwerkgeräts
- Konfiguration der Netzwerksicherheitsgruppen
- Ressourcensperren
- Blockade der erforderlichen Endpunkten

**Fehler**: "Der Remote-PC hat Ihre Sitzung beendet. Wenn dies weiterhin geschieht, wenden Sie sich an Ihren Netzwerkadministrator, um Unterstützung zu erhalten. Fehlercode: 0x3"

**Ursachen**: Dieser Fehler kann auftreten, wenn die Cloud-PC-Workload die Kapazität überschreitet. Wenn das Problem weiterhin besteht, kann es erforderlich sein, den Cloud PC-Arbeitsbereich über das Verwaltungsportal neu zu starten.

Weitere Beispiele für Auslöser für das Nicht-Herstellen einer Verbindung mit dem Cloud-PC sind:

- Es werden keine aktuellen VPN-Clientversionen von Drittanbietern verwendet.
- Der Versuch, sich mit nur AAD-Benutzerkonten beim Cloud-PC anzumelden.
- Verwenden von Client-PCs mit aktiviertem Remote Credential Guard.

Wenn Sie ein Windows 365 Business Kunde sind, lesen Sie [die Informationen zur Problembehandlung Windows 365 Business Probleme beim Einrichten von Cloud-PCs](https://docs.microsoft.com/windows-365/business/troubleshoot-windows-365-business).
Wenn Sie ein Windows 365 Enterprise Kunde sind, lesen Sie [die Informationen zur Problembehandlung Windows 365](https://docs.microsoft.com/windows-365/enterprise/troubleshooting).