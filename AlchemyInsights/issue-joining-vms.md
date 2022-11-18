---
title: Problem beim Verbinden von VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004395"
- "7924"
ms.date: 01/15/2021
ms.openlocfilehash: af312ef94d10e11f9d91b47fb666db16e8b22938
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66405202"
---
# <a name="issue-joining-vms"></a>Problem beim Verbinden von VMs

Führen Sie die folgenden Schritte durch, um Probleme zu beheben, die beim Verbinden von VMs auftreten:

1. Versuchen Sie, sich mit dem **UPN**-Format (z. B. "joeuser@contoso.com") anstelle des **SAMAccountName**-Formats ("CONTOSO\joeuser") anzumelden.
2. Stellen Sie sicher, dass Sie die Kennwortsynchronisierung gemäß den Schritten in der Anleitung *Erste Schritte* aktiviert haben.
3. Stellen Sie sicher, dass das betroffene Benutzerkonto kein externes Konto im Azure AD-Mandanten ist. Externe Benutzer können sich nicht an der verwalteten Domäne anmelden, da Azure AD Domain Services keine Anmeldeinformationen für solche Benutzerkonten hat.
4. Wenn das betroffene Benutzerkonto ein reines Cloud-Benutzerkonto ist, stellen Sie sicher, dass die Benutzer ihr Kennwort geändert haben, nachdem Sie Azure AD Domain Services aktiviert haben. Dieser Schritt bewirkt, dass die für Azure AD Domain Services erforderlichen Anmeldeinformations-Hashes generiert werden.
5. Wenn die betroffenen Benutzerkonten aus einem lokalen Verzeichnis synchronisiert werden, überprüfen Sie, ob die empfohlene Version von Azure AD Connect so konfiguriert wurde, dass eine vollständige Synchronisierung durchgeführt wird.
6. Wenn die Probleme nach der Bestätigung von Schritt 4 weiterhin bestehen, führen Sie die folgenden Befehle von Ihrem Synchronisierungsgerät aus:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.