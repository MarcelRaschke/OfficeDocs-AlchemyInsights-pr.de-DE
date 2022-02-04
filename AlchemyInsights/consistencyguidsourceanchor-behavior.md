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
ms.openlocfilehash: ee0d14276351be472e49500b917f59bf6c476c1a
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61948355"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-Verhalten

Azure AD Verbinden (Version 1.1.524.0 und danach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Verbinden die Synchronisierungsregeln automatisch wie folgt:
  
- Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für jedes lokale AD-Benutzerobjekt, dessen MsDS-ConsistencyGuid-Attribut nicht ausgefüllt ist, schreibt Azure AD Verbinden seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory. Nachdem das Attribut msDS-ConsistencyGuid aufgefüllt wurde, exportiert Azure AD Verbinden das Objekt dann in Azure AD.
    
 **Hinweis:** Sobald ein lokales AD-Objekt in Azure AD Verbinden importiert wurde (d. h. in den AD Connector Space importiert und in das Metaverse projiziert wird), können Sie seinen sourceAnchor-Wert nicht mehr ändern. Um den sourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Verbinden importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie unter: [Azure AD Verbinden: Designkonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

