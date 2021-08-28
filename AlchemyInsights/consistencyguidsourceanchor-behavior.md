---
title: ConsistencyGuid/sourceAnchor-Verhalten
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044339"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-Verhalten

Azure AD Verbinden (Version 1.1.524.0 und danach) erleichtert jetzt die Verwendung von msDS-ConsistencyGuid als sourceAnchor-Attribut. Bei Verwendung dieses Features konfiguriert Azure AD Verbinden automatisch die Synchronisierungsregeln für Folgendes:
  
- Verwenden Sie msDS-ConsistencyGuid als sourceAnchor-Attribut für User-Objekte. ObjectGUID wird für andere Objekttypen verwendet.
    
- Für jedes lokale AD User-Objekt, dessen MsDS-ConsistencyGuid-Attribut nicht ausgefüllt ist, schreibt Azure AD Verbinden seinen objectGUID-Wert zurück in das msDS-ConsistencyGuid-Attribut im lokalen Active Directory. Nachdem das Attribut msDS-ConsistencyGuid aufgefüllt wurde, exportiert Azure AD Verbinden das Objekt dann nach Azure AD.
    
 **Hinweis:** Sobald ein lokales AD-Objekt in Azure AD Verbinden importiert wurde (d. h. in den AD Connector Space importiert und in das Metaverse projiziert wird), können Sie seinen sourceAnchor-Wert nicht mehr ändern. Um den sourceAnchor-Wert für ein bestimmtes lokales AD-Objekt anzugeben, konfigurieren Sie das msDS-ConsistencyGuid-Attribut, bevor es in Azure AD Verbinden importiert wird. 
  
Weitere Informationen zu SourceAnchor und ConsistencyGuid finden Sie unter: [Azure AD Verbinden: Designkonzepte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

