---
title: Ablauf des ADFS-Verbundzertifikats
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1300012"
- "645"
ms.date: 04/21/2020
ms.openlocfilehash: 2bc2612016265dc398f3ce151f3e4a6a52ba4ed3
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66313023"
---
# <a name="adfs-federation-certificate-expiring"></a>Ablauf des ADFS-Verbundzertifikats

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (wenn das Modul noch nicht installiert ist). Wechseln Sie dazu zu ["Azure AD mithilfe von Windows PowerShell verwalten](https://aka.ms/aadposh)".

2. Führen Sie die Schritte im Abschnitt "Szenario 1: Das AD FS-Tokensignaturzertifikat ist abgelaufen" des [Fehlers "Problem beim Zugriff auf die Website" von AD FS aus, wenn sich ein Verbundbenutzer bei Microsoft 365, Azure oder Intune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Führen Sie die Schritte zum [Aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Microsoft, Azure oder Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365) aus.

    Weitere Informationen zum Verlängern von Verbundzertifikaten finden Sie unter [Verlängern von Verbundzertifikaten für Microsoft 365 und Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
