---
title: Domänendienstsynchronisierung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: 1746765918ebb2db6df4d7ccb5a644d415e08153
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65735717"
---
# <a name="domain-service-synchronization"></a>Domänendienstsynchronisierung

Objekte und Anmeldeinformationen in einer von Azure Active Directory Domain Services (Azure AD DS) verwalteten Domäne können entweder lokal innerhalb der Domäne erstellt oder von einem Azure Active Directory (Azure AD)-Mandanten synchronisiert werden. Bei der ersten Bereitstellung von Azure AD DS wird eine automatische Unidirektionale Synchronisierung konfiguriert und initiiert, um die Objekte aus Azure AD zu replizieren. Diese unidirektionale Synchronisierung wird weiterhin im Hintergrund ausgeführt, um die verwaltete Azure AD DS-Domäne mit allen Änderungen von Azure AD auf dem neuesten Stand zu halten. Es erfolgt keine Synchronisierung von Azure AD DS zurück zu Azure AD.

Weitere Informationen zur Azure Active Directory Domänendienstsynchronisierung finden Sie unter [Domänendienstsynchronisierung](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).
