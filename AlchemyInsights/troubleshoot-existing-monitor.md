---
title: Problembehandlung für vorhandenen Monitor
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001450"
- "3454"
ms.openlocfilehash: 26d119db13e4b81c2c0c5ffc649a3ee34521efc4
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66345621"
---
# <a name="troubleshoot-an-existing-monitor"></a>Problembehandlung für einen vorhandenen Monitor

Probieren Sie diese Lösungen aus, um Probleme mit einem Monitor zu beheben. 

**Bildschirmanzeige aktualisieren:**

Drücken Sie gleichzeitig die folgenden Tasten: WINDOWS-TASTE+STRG+UMSCHALT+B. Dadurch wird die Kommunikation mit Dem Grafiktreiber aktualisiert. Ihre Monitore blinken kurz und kehren nach ein paar Sekunden zurück.

**Problembehandlung bei der Monitorhardware:**

1. Ziehen Sie das Kabel ab, das Ihren PC mit Ihrem Monitor verbindet, und schließen Sie es wieder an.
2. Trennen Sie alle nicht wesentlichen Geräte von Ihrem PC (z. B. Adapter oder Dockingstationen).

**Wenn Sie kürzlich ein Update auf Ihrem PC installiert haben, können Sie den Anzeigetreiber zurücksetzen:**

1. Wählen Sie **"Start**" aus, geben Sie **den Geräte-Manager** ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.
2. Erweitern Sie den Abschnitt **"Grafikkarten** ", klicken Sie mit der rechten Maustaste auf die Grafikkarte, und wählen Sie **"Eigenschaften**" aus.
3. Navigieren Sie zur Registerkarte **"Treiber** ", und wählen Sie **"Treiber zurücksetzen" aus**. <br>
Hinweis: Wenn dies nicht verfügbar oder abgeblendet ist, wählen Sie " **Nein** " aus den folgenden Optionen aus, um zum nächsten Schritt zu wechseln.
4. Möglicherweise müssen Sie Ihren PC neu starten, bevor diese Änderungen wirksam werden.

**Deinstallieren Sie den Anzeigetreiber, und installieren Sie den Treiber neu:**

1. Wählen Sie **"Start**" aus, geben Sie **den Geräte-Manager** ein, und wählen Sie in den Ergebnissen **Geräte-Manager** aus.
2. Erweitern Sie den Abschnitt **"Grafikkarten** ", klicken Sie mit der rechten Maustaste auf Ihre Grafikkarte, und wählen Sie " **Gerät deinstallieren" aus**. 
3. Aktivieren Sie das Kontrollkästchen neben **"Treibersoftware für dieses Gerät löschen** ", und wählen Sie **"Deinstallieren"** aus.<br>
Hinweis: Sie werden möglicherweise aufgefordert, Ihren Computer zu diesem Zeitpunkt neu zu starten. Notieren Sie sich vor dem Neustart unbedingt die restlichen Anweisungen.
4. Öffnen Sie Geräte-Manager erneut.
5. Erweitern Sie den Abschnitt **"Grafikkarten** ", klicken Sie mit der rechten Maustaste auf die Grafikkarte, und wählen Sie **"Treiber aktualisieren"** aus.
6. Wählen Sie **"Automatisch nach Updatetreibersoftware suchen** " aus, und folgen Sie den Installationsanweisungen.