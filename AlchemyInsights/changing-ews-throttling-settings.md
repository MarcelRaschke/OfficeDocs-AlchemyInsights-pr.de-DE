---
title: Ändern der Einstellungen für die EWS-Drosselung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4035154c449778d77b9e456099bb07ab00bdce00
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66369795"
---
# <a name="changing-ews-throttling-settings"></a>Ändern der Einstellungen für die EWS-Drosselung

Führen Sie unseren automatisierten Test aus, der es Ihnen ermöglicht, die EWS-Drosselungsrichtlinie für die Dauer der Migration zu ändern. Beachten Sie, dass EWS-Importe auch nach dieser Ausführung weiterhin auf 150 MB pro 5 Minuten pro Postfach beschränkt sind. Um eine höhere Migrationsdurchsatzgeschwindigkeit zu erreichen, sollten Sie mehrere Benutzer gleichzeitig migrieren.

Bitte beachten Sie, dass die Änderungen an der EWS-Einschränkungsrichtlinie sich nicht auf die folgenden Migrationstypen (mit Microsoft-Tools) auswirken: "Hybrid", "Cutover/inszeniert (RPC/HTTP)", "IMAP", "G Suite", "Public Folder" oder "PST Import Service".