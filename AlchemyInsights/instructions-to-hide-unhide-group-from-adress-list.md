---
title: Anweisungen zum Ausblenden/Einblenden von Gruppen in der Adressliste
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
- "1200024"
- "3161"
ms.openlocfilehash: 03a768f2b5bdd92c2dfcf68b6b0d6270878d81c7
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62720997"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ausblenden Microsoft 365 Gruppe aus der Adressliste (GAL)

Um eine Microsoft 365 Gruppe aus Adresslisten (GAL) von Exchange Clients (z. B. Outlook oder OWA) auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Um die Microsoft 365 Gruppe für Exchange Clients auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

