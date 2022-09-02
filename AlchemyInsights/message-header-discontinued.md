---
title: X-MS-Exchange-CrossTenant-ID wird ausgehenden E-Mails nicht mehr hinzugefügt.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200009"
- "18179"
ms.openlocfilehash: 0e6ed51610de01da3bdf718eecbd427494eac5d8
ms.sourcegitcommit: 7c650f8e0593bbb15db359384b89550a35ab7707
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2022
ms.locfileid: "67571982"
---
# <a name="x-ms-exchange-crosstenant-id-is-no-longer-added-to-outgoing-email"></a>X-MS-Exchange-CrossTenant-ID wird ausgehenden E-Mails nicht mehr hinzugefügt.

Aus Datenschutzgründen ist der Nachrichtenkopf "X-MS-Exchange-CrossTenant-id" nicht mehr in ausgehenden Nachrichten enthalten. Dieser Header ist ausschließlich für interne Microsoft 365-Zwecke konzipiert. Interne Kopfzeilen können ohne vorherige Ankündigung eingestellt oder gelöscht werden.

Wenn Sie diese Kopfzeile zum Sperren Ihrer lokalen Umgebung verwenden, lesen Sie [Advanced Office 365 Routing: Sperren des lokalen Exchange,wenn MX auf Office 365 verweist](https://techcommunity.microsoft.com/t5/exchange-team-blog/advanced-office-365-routing-locking-down-exchange-on-premises/ba-p/609238).

Wenn Sie diesen Header zum Steuern des E-Mail-Routings auf Ihrem Drittanbietergateway verwenden, verwenden Sie einen anderen Nachrichtenkopf anstelle von "X-MS-Exchange-CrossTenant-id".