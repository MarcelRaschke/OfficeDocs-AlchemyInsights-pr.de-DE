---
title: ConsistencyGuid/sourceAnchor-Verhalten
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
ms.openlocfilehash: 1de65c9d4797f5027590fc9b30e423c17ddd7af8
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66288838"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-Verhalten

Azure AD Connect (Version 1.1.524.0 und danach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Connect die Synchronisierungsregeln automatisch für:
  
- Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für jedes lokale AD-Benutzerobjekt, dessen msDS-ConsistencyGuid-Attribut nicht aufgefüllt ist, schreibt Azure AD Connect seinen objectGUID-Wert zurück in das Attribut "msDS-ConsistencyGuid" in lokales Active Directory. Nachdem das attribut msDS-ConsistencyGuid aufgefüllt wurde, exportiert Azure AD Connect das Objekt in Azure AD.
    
 **Hinweis:** Nachdem ein lokales AD-Objekt in Azure AD Connect importiert wurde (d. h. in den AD Connector Space importiert und in das Metaverse projiziert wurde), können Sie seinen sourceAnchor-Wert nicht mehr ändern. Um den SourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das attribut msDS-ConsistencyGuid, bevor es in Azure AD Connect importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie unter: [Azure AD Connect: Designkonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

