---
title: Domänendienstsynchronisierung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.date: 01/15/2021
ms.openlocfilehash: e4c97a5a86bdde349d8045260f66a81bf8b77cfd
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66510447"
---
# <a name="domain-service-synchronization"></a>Domänendienstsynchronisierung

Objekte und Anmeldeinformationen in einer von Azure Active Directory Domain Services (Azure AD DS) verwalteten Domäne können entweder lokal innerhalb der Domäne erstellt oder von einem Azure Active Directory (Azure AD)-Mandanten synchronisiert werden. Bei der ersten Bereitstellung von Azure AD DS wird eine automatische Unidirektionale Synchronisierung konfiguriert und initiiert, um die Objekte aus Azure AD zu replizieren. Diese unidirektionale Synchronisierung wird weiterhin im Hintergrund ausgeführt, um die verwaltete Azure AD DS-Domäne mit allen Änderungen von Azure AD auf dem neuesten Stand zu halten. Es erfolgt keine Synchronisierung von Azure AD DS zurück zu Azure AD.

Weitere Informationen zur Azure Active Directory-Domänendienstsynchronisierung finden Sie unter [Domänendienstsynchronisierung](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).
