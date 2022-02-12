---
title: Ändern der Einstellungen für die EWS-Drosselung
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 08c56e376945804bfd2606c9794c664e97b928d5
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62608439"
---
# <a name="changing-ews-throttling-settings"></a>Ändern der Einstellungen für die EWS-Drosselung

Führen Sie unseren automatisierten Test aus, der es Ihnen ermöglicht, die EWS-Drosselungsrichtlinie für die Dauer der Migration zu ändern. Beachten Sie, dass EWS-Importe auch nach dieser Ausführung weiterhin auf 150 MB pro 5 Minuten pro Postfach beschränkt sind. Um eine höhere Migrationsdurchsatzgeschwindigkeit zu erreichen, sollten Sie mehrere Benutzer gleichzeitig migrieren.

Bitte beachten Sie, dass die Änderungen an der EWS-Einschränkungsrichtlinie sich nicht auf die folgenden Migrationstypen (mit Microsoft-Tools) auswirken: "Hybrid", "Cutover/inszeniert (RPC/HTTP)", "IMAP", "G Suite", "Public Folder" oder "PST Import Service".