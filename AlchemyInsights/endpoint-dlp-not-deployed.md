---
title: Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 0512511e00f0b793c1cc25ce49b0679d38c7df08
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63129377"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt

Wenn die Einstellung für die Verhinderung von Datenverlust am Endpunkt nicht auf das Gerät eines Benutzers angewendet wurde, stellen Sie sicher, dass Sie die folgenden Kriterien erfüllt sind:

- Auf dem Gerät ist Windows 10 x64, Build 1809 oder höher, installiert.
- Antischadsoftware-Client, Version 4.18.2009.7 oder höher, ist installiert.
- Auf das Gerät trifft **einer** der folgenden Punkte zu:
    
    - Es ist in Azure Active Directory (Azure AD) eingebunden
    - Es ist in Azure AD Hybrid eingebunden
    - Es ist in AAD registriert

- Um Richtlinienaktionen durchzusetzen, stellen Sie sicher, dass der Microsoft Chromium Edge-Browser auf dem Endpunktgerät installiert ist.

Weitere Anforderungen für die Bereitstellung der Verhinderung von Datenverlust am Endpunkt finden Sie unter [Erste Schritte mit der Verhinderung von Datenverlust am Endpunkt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).