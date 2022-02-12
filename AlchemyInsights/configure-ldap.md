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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 9e6a52116c2f73d6e1b232ae807f59026553febc
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62737505"
---
# <a name="configure-ldap"></a>Konfigurieren von LDAP

Gehen Sie folgendermaßen vor, um LDAP zu konfigurieren:

1. Überprüfen Sie die Integrität Ihrer Domäne im [Azure-Portal](https://aka.ms/aadds-health).
1. Stellen Sie sicher, dass ein gültiges Azure AD Abonnement verfügbar ist und Azure AD Domänendienste aktiviert wurde.
1. Das zum Aktivieren von sicherem LDAP erforderliche Zertifikat muss von einer vertrauenswürdigen öffentlichen Zertifizierungsstelle bezogen werden oder ein selbstsignes Zertifikat sein.
1. Stellen Sie sicher, dass das Zertifikat den erforderlichen [Richtlinien](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate) entspricht.

**Ungültiges Zertifikat**
1. Führen Sie zum Verlängern eines Zertifikats die Schritte zum Erstellen eines neuen Zertifikats und zum erneuten Laden aus: [Konfigurieren von LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Informationen zum Beheben eines bekannten Problems mit Secure LDAP-Warnungen in Azure Active Directory Domain Services finden Sie unter [Beheben von LDAP-Warnungen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
