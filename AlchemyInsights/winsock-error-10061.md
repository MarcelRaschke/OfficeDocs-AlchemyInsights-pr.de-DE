---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083229"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass Microsoft keinen TCP-Socket (Verbindung) mit dem Zielhost herstellen konnte. Die wahrscheinlichste Ursache für diesen Fehler ist ein Problem mit ihrer Firewallkonfiguration. Überprüfen Sie die folgenden Einstellungen, um das Problem zu beheben:

- Überprüfen Der Firewallkonfiguration mit den Informationen in [Microsoft 365 URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler für Exchange Online Protection (EOP) spezifisch ist, sollten Sie zuvor über eine Änderung der [Exchange Online Protection IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)benachrichtigt worden sein.

- Stellen Sie sicher, dass Ihr Internetdienstanbieter (Internet Service Provider, ISP) den Port nicht blockiert.

- Überprüfen Sie die Smarthost- und Zielservereinstellungen in Ihren Connectors.

Beachten Sie, dass Microsoft 365 *eingehende* Verbindungen nicht auf diese Weise blockiert.
