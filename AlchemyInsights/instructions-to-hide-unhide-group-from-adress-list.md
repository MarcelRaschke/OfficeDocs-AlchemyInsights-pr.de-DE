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
ms.openlocfilehash: c22f34e404720dab4e87a300b3a5a4e7a8bd2b9a
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61872556"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ausblenden Microsoft 365 Gruppe aus der Adressliste (GAL)

Um eine Microsoft 365 Gruppe aus Adresslisten (GAL) von Exchange Clients (z. B. Outlook oder OWA) auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Um die Microsoft 365 Gruppe für Exchange Clients auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

