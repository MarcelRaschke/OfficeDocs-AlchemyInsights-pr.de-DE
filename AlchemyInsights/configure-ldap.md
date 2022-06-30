---
title: Konfigurieren von LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004394"
- "7923"
ms.date: 01/15/2021
ms.openlocfilehash: 376a52c7e334aa434c97216bff9136412dc0c59e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66423508"
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
