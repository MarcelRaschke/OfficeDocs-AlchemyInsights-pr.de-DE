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
ms.localizationpriority: medium
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 48d9967112149c2cd4e7065c9eca897b70f67a63
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65732034"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass Microsoft keinen TCP-Socket (Verbindung) mit dem Zielhost herstellen konnte. Die wahrscheinlichste Ursache dieses Fehlers ist ein Problem mit Ihrer Firewallkonfiguration. Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:

- Überprüfen Der Firewallkonfiguration mit den Informationen in [Microsoft 365 URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler für Exchange Online Protection (EOP) spezifisch ist, sollten Sie zuvor über eine Änderung der [Exchange Online Protection IP-Adressen](https://docs.microsoft.com/microsoft-365/security/office-365-security/exchange-online-protection-overview) benachrichtigt worden sein.

- Stellen Sie sicher, dass ihr Internetdienstanbieter (Internet Service Provider, ISP) den Port nicht blockiert.

- Überprüfen Sie die Smarthost- und Zielservereinstellungen in Ihren Connectors.

Beachten Sie, dass Microsoft 365 *eingehende* Verbindungen nicht auf diese Weise blockiert.
