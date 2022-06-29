---
title: Error AttributeValueMustBeUnique
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.date: 04/21/2020
ms.openlocfilehash: 6910dae57c3c1cb5fa3b6c9814e3b5c238f98753
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66269920"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler ist, dass zwei Objekte mit unterschiedlichen SourceAnchor-Attributen (immutableId) denselben Wert für die Attribute "ProxyAddresses" und/oder "UserPrincipalName" aufweisen. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie die duplizierten proxyAddresses, userPrincipalName oder einen anderen Attributwert, der den Fehler verursacht. Identifizieren Sie außerdem, welche zwei (oder mehr) Objekte am Konflikt beteiligt sind. Der von Azure AD Connect Health für die Synchronisierung generierte Bericht kann Ihnen helfen, die beiden Objekte zu identifizieren.
    
2. Identifizieren Sie, welches Objekt weiterhin über den duplizierten Wert verfügen soll und welches nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das NICHT über diesen Wert verfügen sollte. Beachten Sie, dass Sie die Änderung im Verzeichnis vornehmen sollten, aus dem das Objekt stammt. In einigen Fällen müssen Sie möglicherweise eines der in Konflikt stehenden Objekte löschen.
    
4. Wenn Sie die Änderung im lokalen AD vorgenommen haben, lassen Sie Azure AD Connect die Änderung synchronisieren, damit der Fehler behoben wird.
    

