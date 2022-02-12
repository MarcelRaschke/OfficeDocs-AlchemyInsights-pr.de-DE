---
title: Löschen eines privaten Teams-Kanals
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: e2391a9056eab2c551fdb075b848b0b969c1e636
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62556327"
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