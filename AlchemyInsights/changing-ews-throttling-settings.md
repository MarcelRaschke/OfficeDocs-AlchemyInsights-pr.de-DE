---
title: Ändern der Einstellungen für die EWS-Drosselung
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968376"
---
# <a name="changing-ews-throttling-settings"></a>Ändern der Einstellungen für die EWS-Drosselung

Führen Sie unseren automatisierten Test aus, der es Ihnen ermöglicht, die EWS-Drosselungsrichtlinie für die Dauer der Migration zu ändern. Beachten Sie, dass EWS-Importe auch nach dieser Ausführung weiterhin auf 150 MB pro 5 Minuten pro Postfach beschränkt sind. Um eine höhere Migrationsdurchsatzgeschwindigkeit zu erreichen, sollten Sie mehrere Benutzer gleichzeitig migrieren.

Bitte beachten Sie, dass die Änderungen an der EWS-Einschränkungsrichtlinie sich nicht auf die folgenden Migrationstypen (mit Microsoft-Tools) auswirken: "Hybrid", "Cutover/inszeniert (RPC/HTTP)", "IMAP", "G Suite", "Public Folder" oder "PST Import Service".