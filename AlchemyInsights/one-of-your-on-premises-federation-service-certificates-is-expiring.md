---
title: Eines Ihrer lokalen Verbunddienstzertifikate läuft ab
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.date: 04/21/2020
ms.openlocfilehash: 98533df1c88c981ef56d87d73b9b09d631274af6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66256438"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Eines Ihrer lokalen Verbunddienstzertifikate läuft ab

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
- Installieren Sie das Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (wenn das Modul noch nicht installiert ist). Wechseln Sie dazu zu [Azure Active Directory PowerShell für Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0&preserve-view=true).
    
- Führen Sie die Schritte im Abschnitt "Szenario 1: Das AD FS-Tokensignaturzertifikat ist abgelaufen" des [Fehlers "Problem beim Zugriff auf die Website" von AD FS aus, wenn sich ein Verbundbenutzer bei Microsoft 365, Azure oder Intune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Führen Sie die Schritte unter ["Aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Microsoft 365, Azure oder Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)" aus.
    
Weitere Informationen zum Erneuern von Verbundzertifikaten finden Sie unter [Zertifikatverlängerung für O365 und Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
