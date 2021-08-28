---
title: Anweisungen zum Ausblenden/Einblenden von Gruppen in der Adressliste
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926244"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ausblenden Microsoft 365 Gruppe aus der Adressliste (GAL)

Um eine Microsoft 365 Gruppe aus Adresslisten (GAL) von Exchange Clients (z. B. Outlook oder OWA) auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Um die Microsoft 365 Gruppe für Exchange Clients auszublenden, verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

