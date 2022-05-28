---
title: Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.date: 05/26/2022
ms.openlocfilehash: a0a4886d30911b194f4156d224351b31c4d75637
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65718081"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt

Wenn die Einstellung für die Verhinderung von Datenverlust am Endpunkt nicht auf das Gerät eines Benutzers angewendet wurde, stellen Sie sicher, dass Sie die folgenden Kriterien erfüllt sind:

- Auf dem Gerät ist Windows 10 x64, Build 1809 oder höher, installiert.
- Antischadsoftware-Client, Version 4.18.2009.7 oder höher, ist installiert.
- Auf das Gerät trifft **einer** der folgenden Punkte zu:

    - Es ist in Azure Active Directory (Azure AD) eingebunden
    - Es ist in Azure AD Hybrid eingebunden
    - Es ist in AAD registriert

- Um Richtlinienaktionen zu erzwingen, stellen Sie sicher, dass die neueste Version von Edge auf dem Endpunktgerät installiert ist.

Weitere Anforderungen für die Bereitstellung der Verhinderung von Datenverlust am Endpunkt finden Sie unter [Erste Schritte mit der Verhinderung von Datenverlust am Endpunkt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).