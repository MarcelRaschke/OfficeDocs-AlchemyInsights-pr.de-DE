---
title: Konfigurieren von LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: bd7016130f3cead99f21cd9e4738c6f33a3bbe24
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65731710"
---
# <a name="configure-ldap"></a>Konfigurieren von LDAP

Gehen Sie wie folgt vor, um LDAP zu konfigurieren:

1. Überprüfen Sie die Integrität Ihrer Domäne auf der [Azure-Portal](https://aka.ms/aadds-health).
1. Stellen Sie sicher, dass ein gültiges Azure AD-Abonnement verfügbar ist und Azure AD Domain Services aktiviert wurde.
1. Das zum Aktivieren von sicherem LDAP erforderliche Zertifikat muss von einer vertrauenswürdigen öffentlichen Zertifizierungsstelle abgerufen werden oder ein selbstsigniertes Zertifikat sein.
1. Stellen Sie sicher, dass das Zertifikat den erforderlichen [Richtlinien entspricht](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Ungültiges Zertifikat**
1. Führen Sie zum Verlängern eines Zertifikats die Schritte zum Erstellen eines neuen Zertifikats und zum erneutenUploaden aus: [Konfigurieren von LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Informationen zum Beheben eines bekannten Problems mit sicheren LDAP-Warnungen in Azure Active Directory Domain Services finden Sie unter [Beheben von LDAP-Warnungen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
