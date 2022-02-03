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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 76a74fc3326a150d60fe90caa5ec796babf47f05
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61932722"
---
# <a name="adfs-federation-certificate-expiring"></a>Ablauf des ADFS-Verbundzertifikats

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (wenn das Modul noch nicht installiert ist). Wechseln Sie dazu zu [Azure AD mithilfe von Windows PowerShell](https://aka.ms/aadposh)verwalten.

2. Führen Sie die Schritte im Abschnitt "Szenario 1: Das AD FS-Tokensignaturzertifikat ist abgelaufen" unter ["Fehler beim Zugriff auf die Website" von AD FS aus aus, wenn sich ein Verbundbenutzer bei Microsoft 365, Azure oder Intune anmeldet.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Führen Sie die Schritte unter [Aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Microsoft, Azure oder Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)aus.

    Weitere Informationen zum Verlängern von Verbundzertifikaten finden Sie unter Erneuern von [Verbundzertifikaten für Microsoft 365 und Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
