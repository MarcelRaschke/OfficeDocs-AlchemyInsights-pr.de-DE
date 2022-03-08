---
title: ConsistencyGuid/sourceAnchor-Verhalten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 0eb94977e4739b29ff627602d37216ec31d2f8eb
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63161239"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-Verhalten

Azure AD Verbinden (Version 1.1.524.0 und danach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut. Wenn Sie dieses Feature verwenden, konfiguriert Azure AD Verbinden die Synchronisierungsregeln automatisch wie folgt:
  
- Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für jedes lokale AD User-Objekt, dessen MsDS-ConsistencyGuid-Attribut nicht ausgefüllt ist, schreibt Azure AD Verbinden seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory. Nachdem das MsDS-ConsistencyGuid-Attribut aufgefüllt wurde, exportiert Azure AD Verbinden das Objekt dann in Azure AD.
    
 **Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Verbinden importiert wurde (d. h. in den AD-Connectorbereich importiert und in das Metaverse projiziert wird), können Sie seinen sourceAnchor-Wert nicht mehr ändern. Um den sourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Verbinden importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie unter: [Azure AD Verbinden: Designkonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

