---
title: Suchen und Löschen/Löschen von Nachrichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9011283"
- "18297"
ms.openlocfilehash: 4857c98ce55fd93dc39ca0c569d11c6ecbf011fb
ms.sourcegitcommit: 9957d67791fbbf41dad87d8f68b80b24ad5ff842
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2022
ms.locfileid: "67726908"
---
# <a name="search-and-purgedelete-messages"></a>Suchen und Löschen/Löschen von Nachrichten

Sie können nachrichten mit eDiscovery suchen und löschen/löschen. Nachdem Sie eine eDiscovery-Suche ausgeführt haben, um die Nachrichten zu finden, können Sie mithilfe des [Powershell-Befehlslets](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell) `New-ComplianceSearchAction -Purge` bis zu 10 Nachrichten gleichzeitig entfernen.

**Hinweis**: Das Befehlslet kann nicht zum Löschen von Inhalten in SharePoint und OneDrive verwendet werden.

Sie können Chatnachrichten in Teams auch mithilfe der Schritte in ["Suchen nach und Löschen von Chatnachrichten in Teams" löschen](https://docs.microsoft.com/microsoft-365/compliance/search-and-delete-teams-chat-messages#step-5-purge-chat-messages-from-teams).

Weitere Informationen finden Sie unter:

- [Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) 
- [Suchen und Löschen von Chatnachrichten in Teams](https://docs.microsoft.com/microsoft-365/compliance/search-and-delete-teams-chat-messages)