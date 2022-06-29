---
title: Automatisches Anmelden bei Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004625"
- "9003848"
- "6898"
- "8333"
ms.date: 12/03/2020
ms.openlocfilehash: a350711c8c4d9ecb8c128fbd56ae0c2adf71edc2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66255430"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatisches Anmelden bei Microsoft Edge

Microsoft Edge verwendet das Standardkonto des Betriebssystems, um einen Benutzer automatisch entsprechend der Konfiguration des Geräts des Benutzers anzumelden. 

Die Szenarien der einzelnen Gerätekonfigurationstypen und deren abhängiger Benutzeranmeldungsprozess werden im Folgenden beschrieben:

- **Das Gerät ist hybrid/AAD-J**: Diese Option ist in Windows 10- und Windows-Vorgängerversionen und entsprechenden Serverversionen verfügbar. Benutzer werden automatisch mit ihren Azure Active Directory (AD)-Konten angemeldet.
- **Das Gerät ist in die Domäne eingebunden**: Diese Option ist in Windows 10- und Windows-Versionen auf unterer Ebene und entsprechenden Serverversionen verfügbar. Standardmäßig werden Benutzer mit Domänenkonten nicht automatisch angemeldet. um die automatische Anmeldung für sie zu aktivieren, verwenden Sie die **ConfigureOnPremisesAccountAutoSignIn-Richtlinie** . Um die automatische Anmeldung für Benutzer mit Azure AD-Konten zu aktivieren, sollten Sie eine Hybridverbindung zu ihren Geräten in Betracht ziehen.
- **Das Standardkonto des Betriebssystems ist ein Microsoft-Konto**: Diese Option ist auf Windows 10 RS3 (Version 1709, Build 10.0.16299) und höheren Versionen verfügbar. Das Szenario wird auf Unternehmensgeräten wahrscheinlich nicht auftreten. Wenn das Standardkonto des Betriebssystems jedoch ein Microsoft-Konto ist, wird microsoft Edge den Benutzer automatisch mit dem Microsoft-Konto anmelden.
 
 
