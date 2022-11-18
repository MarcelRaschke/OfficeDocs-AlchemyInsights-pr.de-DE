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
ms.custom:
- "9000292"
- "11470"
ms.date: 05/26/2022
ms.openlocfilehash: cb16f6e11edd50edace9e0ff8733fb8982d31115
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66259102"
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