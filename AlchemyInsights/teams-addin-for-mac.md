---
title: Teams-Add-in für Mac
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 4c6023f24307dd237f342d8f9a07cf2bc2d81079
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61970311"
---
# <a name="teams-add-in-for-mac"></a>Teams-Add-in für Mac

Führen Sie die folgenden Schritte aus, um ein fehlendes Team-Add-in für Benutzende des Mac-Betriebssystems zu beheben:

**Schritt 1:** Wenn Sie über Hybrid Exchange On-Premises verfügen (2016 CU3 oder höher erforderlich), verwenden Sie das Tool Test-HMA.ps1, um zu bestätigen, dass die Hybrid Modern Authentication korrekt konfiguriert ist. Weitere Informationen finden Sie unter [Hybrid Modern Authentication für Outlook für iOS und Android validieren](https://aka.ms/TestHMAEAS).  

**Hinweis** verwenden Sie das UPN-Adressformat (beispielsweise [username@contoso.com](mailto:username@contoso.com)), nicht domain\username. Tun Sie dies auch für Benutzende mit Exchange Online-Postfächern.

**Schritt 2:** Lassen Sie Benutzende in Outlook für Mac auf **Tools** > **Konten** gehen und das Konto suchen und auswählen. Bestätigen Sie, dass der aufgelistete Benutzername im UPN-Format (beispielsweise [username@contoso.com](mailto:username@contoso.com)) ist.

**Schritt 3:** Bestätigen Sie, dass die Benutzenden lizenzierte Microsoft Teams-Benutzende sind. Benutzende müssen das Office 365 für Mac-Abonnement, Produktversion 16.24 oder höher, verwenden.