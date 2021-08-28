---
title: Teams-Add-in für Mac
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940674"
---
# <a name="teams-add-in-for-mac"></a>Teams-Add-in für Mac

Führen Sie die folgenden Schritte aus, um ein fehlendes Team-Add-in für Benutzende des Mac-Betriebssystems zu beheben:

**Schritt 1:** Wenn Sie über Hybrid Exchange On-Premises verfügen (2016 CU3 oder höher erforderlich), verwenden Sie das Tool Test-HMA.ps1, um zu bestätigen, dass die Hybrid Modern Authentication korrekt konfiguriert ist. Weitere Informationen finden Sie unter [Hybrid Modern Authentication für Outlook für iOS und Android validieren](https://aka.ms/TestHMAEAS).  

**Hinweis** verwenden Sie das UPN-Adressformat (beispielsweise [username@contoso.com](mailto:username@contoso.com)), nicht domain\username. Tun Sie dies auch für Benutzende mit Exchange Online-Postfächern.

**Schritt 2:** Lassen Sie Benutzende in Outlook für Mac auf **Tools** > **Konten** gehen und das Konto suchen und auswählen. Bestätigen Sie, dass der aufgelistete Benutzername im UPN-Format (beispielsweise [username@contoso.com](mailto:username@contoso.com)) ist.

**Schritt 3:** Bestätigen Sie, dass die Benutzenden lizenzierte Microsoft Teams-Benutzende sind. Benutzende müssen das Office 365 für Mac-Abonnement, Produktversion 16.24 oder höher, verwenden.