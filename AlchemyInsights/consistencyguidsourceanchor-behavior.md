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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 510c1ff7d4c20e4e1aa0270515ad6f727adc1d96
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62671063"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-Verhalten

Azure AD Verbinden (Version 1.1.524.0 und danach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Verbinden automatisch die Synchronisierungsregeln für Folgendes:
  
- Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für jedes lokale AD User-Objekt, dessen msDS-ConsistencyGuid-Attribut nicht ausgefüllt ist, schreibt Azure AD Verbinden seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory. Nachdem das MsDS-ConsistencyGuid-Attribut aufgefüllt wurde, exportiert Azure AD Verbinden das Objekt dann in Azure AD.
    
 **Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Verbinden importiert wurde (d. h. in den AD Connector Space importiert und in das Metaverse projiziert wird), können Sie seinen sourceAnchor-Wert nicht mehr ändern. Um den sourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Verbinden importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie unter: [Azure AD Verbinden: Designkonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

