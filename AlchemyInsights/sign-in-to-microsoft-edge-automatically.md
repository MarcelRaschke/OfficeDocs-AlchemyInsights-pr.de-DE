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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4a715bc892dc7a1295b6e38e6ed7d3962ee11bbb
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62632326"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatische Anmeldung bei Microsoft Edge

Microsoft Edge verwendet das Standardkonto des Betriebssystems, um einen Benutzer automatisch entsprechend der Konfiguration des Geräts des Benutzers anzumelden. 

Die Szenarien der einzelnen Gerätekonfigurationstypen und deren abhängiger Benutzeranmeldungsprozess werden im Folgenden beschrieben:

- **Das Gerät ist hybrid/AAD-J**: Diese Option ist in Windows 10, Windows auf der unteren Ebene und den entsprechenden Serverversionen verfügbar. Benutzer werden automatisch mit ihren Azure Active Directory (AD)-Konten angemeldet.
- **Das Gerät ist in die Domäne eingebunden**: Diese Option ist in Windows 10, Windows auf der unteren Ebene und den entsprechenden Serverversionen verfügbar. Standardmäßig sind Benutzer mit Domänenkonten nicht automatisch angemeldet. Um die automatische Anmeldung für sie zu aktivieren, verwenden **Sie die ConfigureOnPremisesAccountAutoSignIn-Richtlinie** . Um die automatische Anmeldung für Benutzer mit Azure AD Konten zu aktivieren, sollten Sie die Hybridverbindung ihrer Geräte in Betracht ziehen.
- **Das Standardkonto des Betriebssystems ist ein Microsoft-Konto**: Diese Option ist in Windows 10 RS3 (Version 1709, Build 10.0.16299) und höher verfügbar. Es ist unwahrscheinlich, dass das Szenario auf Unternehmensgeräten auftritt. Wenn das Standardkonto des Betriebssystems jedoch ein Microsoft-Konto ist, melden Microsoft Edge den Benutzer automatisch mit dem Microsoft-Konto an.
 
 
