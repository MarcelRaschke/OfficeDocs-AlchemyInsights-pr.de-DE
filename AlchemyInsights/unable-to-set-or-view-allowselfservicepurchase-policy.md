---
title: Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: f0ea23156ee34636de83b55e09e36eace843ef25
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66344685"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden.

Beim Versuch, die AllowSelfServicePurchase-Richtlinie festzulegen oder anzuzeigen, wird die folgende Fehlermeldung angezeigt:

*HandleError: Fehler beim Abrufen der Produktrichtlinie mit der PolicyId "AllowSelfServicePurchase", ErrorMessage - Die zugrunde liegende Verbindung wurde geschlossen: Unerwarteter Fehler beim Senden.*

Dies kann auf eine ältere Version von Transport Layer Security (TLS) zurückzuführen sein. Um den MSCommerce-Dienst zu verbinden, müssen Sie TLS 1.2 oder höher verwenden.  

Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1.2 zu aktivieren/festlegen, zu überprüfen und erneut zu versuchen.
 1. Geben Sie an der PowerShell-Eingabeaufforderung (PS C:\) Geben Sie den folgenden Befehl ein, um das TLS-Protokoll auf Version 1.2 festzulegen:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Überprüfen Sie die verwendeten TLS-Protokolle mit dem folgenden Befehl:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Wiederholen Sie die Befehle "Abrufen" oder "Aktualisieren" nach Bedarf.

