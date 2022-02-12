---
title: Error AttributeValueMustBeUnique
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ff690a5caeccf700c5fe50dbadb442b2cb6c87c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62554743"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler sind zwei Objekte mit unterschiedlichen SourceAnchor -Objekten (immutableId) mit demselben Wert für die ProxyAddresses- und/oder UserPrincipalName-Attribute. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie die duplizierten proxyAddresses, userPrincipalName oder einen anderen Attributwert, der den Fehler verursacht. Identifizieren Sie außerdem, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der von Azure AD Verbinden Health for Sync generierte Bericht kann Ihnen dabei helfen, die beiden Objekte zu identifizieren.
    
2. Identifizieren Sie, welches Objekt weiterhin den duplizierten Wert haben soll und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das diesen Wert NICHT aufweisen sollte. Beachten Sie, dass Sie die Änderung in dem Verzeichnis vornehmen sollten, aus dem das Objekt stammt. In einigen Fällen müssen Sie möglicherweise eines der Objekte löschen, die sich in Konflikt befinden.
    
4. Wenn Sie die Änderung im lokalen AD vorgenommen haben, lassen Sie Azure AD Verbinden die Änderung synchronisieren, damit der Fehler behoben wird.
    

