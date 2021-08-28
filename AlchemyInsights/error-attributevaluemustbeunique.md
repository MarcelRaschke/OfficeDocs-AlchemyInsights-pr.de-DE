---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002119"
---
# <a name="error-attributevaluemustbeunique"></a>Fehler: AttributeValueMustBeUnique

Der häufigste Grund für den AttributeValueMustBeUnique-Fehler sind zwei Objekte mit unterschiedlichen SourceAnchor -Objekten (immutableId) haben den gleichen Wert für die ProxyAddresses- und/oder UserPrincipalName-Attribute. So beheben Sie den AttributeValueMustBeUnique-Fehler:
  
1. Identifizieren Sie die duplizierten proxyAddresses, userPrincipalName oder einen anderen Attributwert, der den Fehler verursacht. Identifizieren Sie außerdem, welche zwei (oder mehr) Objekte an dem Konflikt beteiligt sind. Der von Azure AD Verbinden Health for Sync generierte Bericht kann Ihnen helfen, die beiden Objekte zu identifizieren.
    
2. Identifizieren Sie, welches Objekt weiterhin den duplizierten Wert haben soll und welches Objekt nicht.
    
3. Entfernen Sie den duplizierten Wert aus dem Objekt, das diesen Wert NICHT aufweisen sollte. Beachten Sie, dass Sie die Änderung in dem Verzeichnis vornehmen sollten, aus dem das Objekt stammt. In einigen Fällen müssen Sie möglicherweise eines der Objekte löschen, die sich in Konflikt befinden.
    
4. Wenn Sie die Änderung im lokalen AD vorgenommen haben, lassen Sie Azure AD Verbinden die Änderung synchronisieren, damit der Fehler behoben wird.
    

