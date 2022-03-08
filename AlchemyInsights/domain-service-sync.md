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
ms.openlocfilehash: ea85216eff9adcfe032e264688ca56e5e30a8d16
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63204116"
---
# <a name="domain-service-synchronization"></a>Domänendienstsynchronisierung

Objekte und Anmeldeinformationen in einer verwalteten Domäne Azure Active Directory Domain Services (Azure AD DS) können entweder lokal innerhalb der Domäne erstellt oder von einem Azure Active Directory (Azure AD)-Mandanten synchronisiert werden. Wenn Sie Azure AD DS zum ersten Mal bereitstellen, wird eine automatische unidirektionale Synchronisierung konfiguriert und initiiert, um die Objekte aus Azure AD zu replizieren. Diese unidirektionale Synchronisierung wird weiterhin im Hintergrund ausgeführt, um die Azure AD verwalteten DS-Domäne mit änderungen von Azure AD auf dem neuesten Stand zu halten. Es erfolgt keine Synchronisierung von Azure AD DS zurück zu Azure AD.

Weitere Informationen zu Azure Active Directory Domänendienstsynchronisierung finden Sie unter [Domänendienstsynchronisierung](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
