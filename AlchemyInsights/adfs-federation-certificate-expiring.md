---
title: Ablauf des ADFS-Verbundzertifikats
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: b29fdc18ce7d08453ec8ea1ad6437015fd44fdff
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63242549"
---
# <a name="adfs-federation-certificate-expiring"></a>Ablauf des ADFS-Verbundzertifikats

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (sofern das Modul noch nicht installiert ist). Wechseln Sie dazu zu ["Azure AD mithilfe von Windows PowerShell verwalten](https://aka.ms/aadposh)".

2. Führen Sie die Schritte im Abschnitt "Szenario 1: Das AD FS-Tokensignierungszertifikat ist abgelaufen" unter ["Fehler beim Zugriff auf die Website" von AD FS aus aus, wenn sich ein Verbundbenutzer bei Microsoft 365, Azure oder Intune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Führen Sie die Schritte unter [Aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Microsoft, Azure oder Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365) aus.

    Weitere Informationen zum Verlängern von Verbundzertifikaten finden Sie unter [Erneuern von Verbundzertifikaten für Microsoft 365 und Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
