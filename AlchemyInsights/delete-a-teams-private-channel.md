---
title: Löschen eines privaten Teams-Kanals
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9001223"
- "3781"
ms.date: 07/24/2020
ms.openlocfilehash: c08944d9bf889d725005213e2202fbf21f17441b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66324831"
---
# <a name="delete-a-teams-private-channel"></a>Löschen eines privaten Teams-Kanals

Microsoft ist sich eines Problems beim Löschen eines privaten Teams-Kanals bewusst, wenn Sie für die zugrunde liegende SharePoint-Site SharePoint-Aufbewahrungsrichtlinien aktiviert haben. Microsoft arbeitet derzeit an einer Lösung. In der Zwischenzeit können Sie folgenden Problemumgehungen verwenden, um den privaten Kanal zu löschen.

**Schließen Sie die Team-/Websitesammlung aus der SharePoint-Aufbewahrungsrichtlinie aus.**

1. Wechseln Sie zum Office 365-Verwaltungsportal, und wählen Sie im linken Navigationsbereich **Alle anzeigen** aus.
2. Wechseln Sie unter **Admin Center** zu **Security & Compliance** > **Verhinderung von Datenverlust** > **Richtlinie**.
3. Identifizieren Sie eine Richtlinie, die für SharePoint-Sites gilt, und ändern Sie die Richtlinie so, dass die SharePoint-Site für das Team, das den privaten Kanal enthält, NICHT unter der Aufbewahrungsrichtlinie enthalten ist.
4. Speichern Sie die Richtlinie.
    Es kann bis zu 24 Stunden dauern, bis Richtlinieneinstellungen wirksam werden.
    Nachdem die Site ausgeschlossen wurde, können Sie den privaten Kanal löschen.  
    
***Möglicherweise können*** Sie den privaten Kanal löschen, indem Sie Microsoft Teams auf Ihrem Android-Gerät verwenden. 

Verwandte SharePoint-Informationen finden Sie unter [Elemente in SharePoint Online oder OneDrive for Business können nicht gelöscht werden](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).