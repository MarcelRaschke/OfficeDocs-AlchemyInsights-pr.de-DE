---
title: Anweisungen zum Ausblenden/Einblenden von Gruppen in der Adressliste
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 04093370114b4b470fb71fd696bb91da9dff78e9
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66405760"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ausblenden der Microsoft 365-Gruppe in der Adressliste (GAL)

Verwenden Sie den folgenden Befehl in der EXO-Shell, um eine Microsoft 365-Gruppe in Adresslisten (GAL) von Exchange-Clients (z. B. Outlook oder OWA) auszublenden:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Zum Ausblenden der Microsoft 365-Gruppe für Exchange-Clients verwenden Sie den folgenden Befehl in der EXO-Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

