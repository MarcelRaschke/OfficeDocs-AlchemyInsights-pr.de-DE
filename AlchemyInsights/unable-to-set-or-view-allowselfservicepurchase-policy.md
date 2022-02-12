---
title: AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden
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
- "9001212"
- "3526"
ms.openlocfilehash: 50a21f64a70e738e663edebf9ffc113404a58059
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62749236"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden

Beim Versuch, die AllowSelfServicePurchase-Richtlinie festzulegen oder anzuzeigen, wird die folgende Fehlermeldung angezeigt:

*HandleError: Fehler beim Abrufen der Produktrichtlinie mit "AllowSelfServicePurchase", ErrorMessage : Die zugrunde liegende Verbindung wurde geschlossen: Beim Senden ist ein unerwarteter Fehler aufgetreten.*

Dies kann auf eine ältere Version von Transport Layer Security (TLS) zurückzuführen sein. Um den MSTeroperabilität-Dienst zu verbinden, müssen Sie TLS 1.2 oder höher verwenden.  

Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1.2 zu aktivieren/festzulegen, es zu überprüfen und erneut zu versuchen.
 1. Geben Sie an der PowerShell-Eingabeaufforderung (PS C:\) Geben Sie den folgenden Befehl ein, um das TLS-Protokoll auf Version 1.2 festzulegen:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Überprüfen Sie die verwendeten TLS-Protokolle mit dem folgenden Befehl:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Wiederholen Sie die Befehle "Abrufen" oder "Aktualisieren" nach Bedarf.

