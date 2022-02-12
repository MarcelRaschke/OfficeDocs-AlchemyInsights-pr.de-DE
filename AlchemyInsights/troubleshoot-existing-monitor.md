---
title: Problembehandlung bei vorhandenem Monitor
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
- "3454"
- "9001450"
ms.openlocfilehash: ce103210ffaca9305a4a96997f436bc6ed3e5358
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62546155"
---
# <a name="troubleshoot-an-existing-monitor"></a>Problembehandlung für einen vorhandenen Monitor

Probieren Sie diese Lösungen aus, um Probleme mit einem Monitor zu beheben. 

**Aktualisieren Sie die Anzeige Des Monitors:**

Drücken Sie gleichzeitig die folgenden Tasten: Windows Taste + STRG + UMSCHALT + B. Dadurch wird die Kommunikation mit Dem Grafiktreiber aktualisiert. Ihre Monitore blinken kurz und kehren nach ein paar Sekunden zurück.

**Problembehandlung bei der Monitorhardware:**

1. Ziehen Sie das Kabel ab, das Ihren PC mit Ihrem Monitor verbindet, und schließen Sie es wieder an.
2. Trennen Sie alle nicht wesentlichen Geräte von Ihrem PC (z. B. Adapter oder Dockingstationen).

**Wenn Sie kürzlich ein Update auf Ihrem PC installiert haben, können Sie ein Rollback des Anzeigetreibers ausführen:**

1. Wählen Sie **"Start**", geben Sie **"Geräte-Manager**" ein, und wählen Sie " **Geräte-Manager** " aus den Ergebnissen aus.
2. Erweitern Sie den Abschnitt " **Grafikkarten"** , klicken Sie mit der rechten Maustaste auf den Grafikkartenadapter, und wählen Sie " **Eigenschaften**" aus.
3. Navigieren Sie zur Registerkarte **"Treiber** ", und wählen Sie **"Treiber zurücksetzen" aus**. <br>
Hinweis: Wenn dies nicht verfügbar ist oder abgeblendet ist, wählen Sie in den folgenden Optionen **"Nein** " aus, um zum nächsten Schritt zu wechseln.
4. Möglicherweise müssen Sie Ihren PC neu starten, bevor diese Änderungen wirksam werden.

**Deinstallieren Sie den Anzeigetreiber, und installieren Sie ihn neu:**

1. Wählen Sie **"Start**", geben Sie **"Geräte-Manager**" ein, und wählen Sie " **Geräte-Manager** " aus den Ergebnissen aus.
2. Erweitern Sie den Abschnitt " **Grafikkarten"** , klicken Sie mit der rechten Maustaste auf den Grafikkartenadapter, und wählen **Sie "Gerät deinstallieren" aus**. 
3. Aktivieren Sie das Kontrollkästchen neben **"Treibersoftware für dieses Gerät löschen** ", und wählen Sie **"Deinstallieren" aus**.<br>
Hinweis: Möglicherweise werden Sie aufgefordert, Ihren Computer in dieser Phase neu zu starten. Notieren Sie sich unbedingt die restlichen Anweisungen, bevor Sie neu starten.
4. Öffnen Sie den Geräte-Manager erneut.
5. Erweitern Sie den Abschnitt **"Grafikkarten"** , klicken Sie mit der rechten Maustaste auf den Grafikkartenadapter, und wählen Sie " **Treiber aktualisieren" aus**.
6. Wählen Sie **"Suchen" automatisch nach Updatetreibersoftware** aus, und befolgen Sie die Installationsanweisungen.