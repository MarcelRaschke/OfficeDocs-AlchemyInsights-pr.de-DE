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
ms.openlocfilehash: a1fe54e828f220ea69617fad8d7b033b11c3e8ae
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62567919"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass Microsoft keinen TCP-Socket (Verbindung) mit dem Zielhost herstellen konnte. Die wahrscheinlichste Ursache für diesen Fehler ist ein Problem mit ihrer Firewallkonfiguration. Überprüfen Sie die folgenden Einstellungen, um das Problem zu beheben:

- Überprüfen Der Firewallkonfiguration mit den Informationen in [Microsoft 365 URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler für Exchange Online Protection (EOP) spezifisch ist, sollten Sie zuvor über eine Änderung der [Exchange Online Protection IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses) benachrichtigt worden sein.

- Stellen Sie sicher, dass Ihr Internetdienstanbieter (Internet Service Provider, ISP) den Port nicht blockiert.

- Überprüfen Sie die Smarthost- und Zielservereinstellungen in Ihren Connectors.

Beachten Sie, dass Microsoft 365 *eingehende* Verbindungen nicht auf diese Weise blockiert.
