---
title: Eines Ihrer lokalen Verbunddienstzertifikate läuft ab
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: ad54962c2311e5022273683cfe660866c50e5f8c
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63272249"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Eines Ihrer lokalen Verbunddienstzertifikate läuft ab

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
- Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (sofern das Modul noch nicht installiert ist). Wechseln Sie dazu zu [Azure Active Directory PowerShell für Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0&preserve-view=true)
    
- Führen Sie die Schritte im Abschnitt "Szenario 1: Das AD FS-Tokensignaturzertifikat ist abgelaufen" unter ["Fehler beim Zugriff auf die Website" von AD FS aus aus, wenn sich ein Verbundbenutzer bei Microsoft 365, Azure oder Intune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Führen Sie die Schritte in ["Aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Microsoft 365, Azure oder Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)" aus.
    
Weitere Informationen zum Verlängern von Verbundzertifikaten finden Sie unter [Zertifikatverlängerung für O365 und Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
