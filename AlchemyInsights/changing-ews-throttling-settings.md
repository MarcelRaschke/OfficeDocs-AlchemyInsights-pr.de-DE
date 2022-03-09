---
title: Ändern der Einstellungen für die EWS-Drosselung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: e5aafd5f0006435804055b897d5f91314ebdd949
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63258425"
---
# <a name="changing-ews-throttling-settings"></a>Ändern der Einstellungen für die EWS-Drosselung

Führen Sie unseren automatisierten Test aus, der es Ihnen ermöglicht, die EWS-Drosselungsrichtlinie für die Dauer der Migration zu ändern. Beachten Sie, dass EWS-Importe auch nach dieser Ausführung weiterhin auf 150 MB pro 5 Minuten pro Postfach beschränkt sind. Um eine höhere Migrationsdurchsatzgeschwindigkeit zu erreichen, sollten Sie mehrere Benutzer gleichzeitig migrieren.

Bitte beachten Sie, dass die Änderungen an der EWS-Einschränkungsrichtlinie sich nicht auf die folgenden Migrationstypen (mit Microsoft-Tools) auswirken: "Hybrid", "Cutover/inszeniert (RPC/HTTP)", "IMAP", "G Suite", "Public Folder" oder "PST Import Service".