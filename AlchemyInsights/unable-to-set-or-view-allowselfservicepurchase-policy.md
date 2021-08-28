---
title: AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020191"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden

Beim Versuch, die AllowSelfServicePurchase-Richtlinie festzulegen oder anzuzeigen, wird die folgende Fehlermeldung angezeigt:

*HandleError: Fehler beim Abrufen der Produktrichtlinie mit "AllowSelfServicePurchase", ErrorMessage : Die zugrunde liegende Verbindung wurde geschlossen: Beim Senden ist ein unerwarteter Fehler aufgetreten.*

Dies kann auf eine ältere Version von Transport Layer Security (TLS) zurückzuführen sein. Um den MSTeroperabilität-Dienst zu verbinden, müssen Sie TLS 1.2 oder höher verwenden.  

Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1.2 zu aktivieren/festzulegen, es zu überprüfen und erneut zu versuchen.
 1. Geben Sie an der PowerShell-Eingabeaufforderung (PS C: \) Geben Sie den folgenden Befehl ein, um das TLS-Protokoll auf Version 1.2 festzulegen:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Überprüfen Sie die verwendeten TLS-Protokolle mit dem folgenden Befehl:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Wiederholen Sie die Befehle "Abrufen" oder "Aktualisieren" nach Bedarf.

