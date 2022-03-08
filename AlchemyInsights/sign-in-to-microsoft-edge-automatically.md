---
title: Automatische Anmeldung bei Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 7b1f52002c53072840d7ef674213d330e9036fbb
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63179888"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatische Anmeldung bei Microsoft Edge

Microsoft Edge verwendet das Standardkonto des Betriebssystems, um einen Benutzer automatisch entsprechend der Konfiguration des Geräts des Benutzers anzumelden. 

Die Szenarien der einzelnen Gerätekonfigurationstypen und deren abhängiger Benutzeranmeldungsprozess werden im Folgenden beschrieben:

- **Das Gerät ist hybrid/AAD-J**: Diese Option ist in Windows 10, Windows und entsprechenden Serverversionen verfügbar. Benutzer werden automatisch mit ihren Azure Active Directory (AD)-Konten angemeldet.
- **Das Gerät ist in die Domäne eingebunden**: Diese Option ist auf Windows 10, auf der unteren Ebene Windows und den entsprechenden Serverversionen verfügbar. Standardmäßig sind Benutzer mit Domänenkonten nicht automatisch angemeldet. Um die automatische Anmeldung für sie zu aktivieren, verwenden **Sie die ConfigureOnPremisesAccountAutoSignIn-Richtlinie** . Um die automatische Anmeldung für Benutzer mit Azure AD Konten zu aktivieren, sollten Sie die Hybridverbindung ihrer Geräte in Betracht ziehen.
- **Das Standardkonto des Betriebssystems ist ein Microsoft-Konto**: Diese Option ist in Windows 10 RS3 (Version 1709, Build 10.0.16299) und höher verfügbar. Es ist unwahrscheinlich, dass das Szenario auf Unternehmensgeräten auftritt. Wenn das Standardkonto des Betriebssystems jedoch ein Microsoft-Konto ist, wird Microsoft Edge den Benutzer automatisch mit dem Microsoft-Konto anmelden.
 
 
