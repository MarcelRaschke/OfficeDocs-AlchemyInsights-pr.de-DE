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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: cc5108798133f3f1b55aeb7451dd9943aabffc66
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62735525"
---
# <a name="domain-service-synchronization"></a>Domänendienstsynchronisierung

Objekte und Anmeldeinformationen in einer verwalteten Domäne Azure Active Directory Domain Services (Azure AD DS) können entweder lokal innerhalb der Domäne erstellt oder von einem Azure Active Directory (Azure AD)-Mandanten synchronisiert werden. Wenn Sie Azure AD DS zum ersten Mal bereitstellen, wird eine automatische unidirektionale Synchronisierung konfiguriert und initiiert, um die Objekte aus Azure AD zu replizieren. Diese unidirektionale Synchronisierung wird weiterhin im Hintergrund ausgeführt, um die Azure AD verwalteten DS-Domäne mit änderungen von Azure AD auf dem neuesten Stand zu halten. Es erfolgt keine Synchronisierung von Azure AD DS zurück zu Azure AD.

Weitere Informationen zu Azure Active Directory Domänendienstsynchronisierung finden Sie unter ["Domänendienstsynchronisierung"](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
