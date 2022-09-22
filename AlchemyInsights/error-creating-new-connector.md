---
title: Fehler beim Erstellen eines neuen Connectors
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
ms.localizationpriority: high
ROBOTS: NOINDEX, NOFOLLOW
ms.custom:
- "9010041"
- "18112"
ms.openlocfilehash: eeeccadd41eeb1862cc829bfdddf29bd4ea15c85
ms.sourcegitcommit: d338792da6b805af409be857cf2e4794fd1550ef
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2022
ms.locfileid: "67883332"
---
# <a name="error-while-creating-new-connector"></a>Fehler beim Erstellen eines neuen Connectors

**Problem**: Beim Versuch, einen Exchange-Connector für "Eingehend zu 365" zu erstellen, wird der Connector nicht erstellt, und Möglicherweise wird die Fehlermeldung "Fehler beim Erstellen des Connectors: Antwortinhalt ist Null" angezeigt.

**Lösung**: Wir untersuchen das Problem. Verwenden Sie Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps), um den Connector zu erstellen.

Verwenden Sie zum Erstellen eines neuen eingehenden Connectors das Cmdlet [New-InboundConnector](https://docs.microsoft.com/powershell/module/exchange/new-inboundconnector?view=exchange-ps) .

Verwenden Sie zum Bearbeiten eines vorhandenen Connectors das Cmdlet [Set-InboundConnector](https://docs.microsoft.com/powershell/module/exchange/set-inboundconnector?view=exchange-ps) .

Beispiel:

`New-InboundConnector -Name "Contoso Inbound Connector" -SenderDomains *.contoso.com -SenderIPAddresses 192.168.0.1/25 -RestrictDomainsToIPAddresses $true`

Der obige Befehl erstellt den eingehenden Connector namens Contoso Inbound Connector mit den folgenden Eigenschaften:

- Lauscht auf eingehende Verbindungen von der Domäne contoso.com und allen Unterdomänen.
- Akzeptiert E-Mails nur von contoso.com und aus dem IP-Bereich 192.168.0.1/25. E-Mails von contoso.com werden abgelehnt, wenn die E-Mail von einer anderen IP-Adresse stammt.