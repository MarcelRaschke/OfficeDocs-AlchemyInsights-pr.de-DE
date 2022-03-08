---
title: Anweisungen zum Ausblenden/Einblenden von Gruppen in der Adressliste
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 942ef57d7ab252df2d75a56c9075200f7d3b45de
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63265157"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ausblenden Microsoft 365 Gruppe aus der Adressliste (GAL)

Um eine Microsoft 365 Gruppe aus Adresslisten (GAL) von Exchange Clients (z. B. Outlook oder OWA) auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Um die Microsoft 365 Gruppe für Exchange Clients auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

