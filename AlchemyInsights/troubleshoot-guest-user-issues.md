---
title: Behandeln von Problemen mit Gastbenutzern
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: d780a446945bcaae143367fa3fb5baad844a28b8
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63209804"
---
# <a name="troubleshoot-guest-user-issues"></a>Behandeln von Problemen mit Gastbenutzern

1. Eine Anleitung zum Verwalten des Gastzugriffs auf Anwendungen finden Sie unter [Verwalten des Gastzugriffs mit Azure AD Zugriffsüberprüfungen](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Hinzufügen von Gastbenutzern zu Ihrem Verzeichnis im Azure-Portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In dieser Schnellstartanleitung fügen Sie ihrem Azure AD Verzeichnis über das Azure-Portal einen neuen Gastbenutzer hinzu, senden eine Einladung und sehen, wie der Einladungseinlösungsprozess des Gastbenutzers aussieht.
1. [Hinzufügen eines Gastbenutzers mit PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In dieser Schnellstartanleitung verwenden Sie den Befehl New-AzureADMSInvitation, um Ihrem Azure-Mandanten einen Gastbenutzer hinzuzufügen.
1. Informationen zum Zuweisen von Benutzern und Gruppen zu Unternehmensanwendungen in Azure Active Directory (Azure AD), entweder im Azure-Portal oder mithilfe von PowerShell, finden Sie unter [Verwalten der Benutzerzuweisung für eine App in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-Zusammenarbeit funktioniert mit den meisten Apps, die in Azure AD integriert sind. In diesem [Artikel](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) werden Anweisungen zum Konfigurieren einiger beliebter SaaS-Apps für die Verwendung mit Azure AD B2B erläutert.
1. Als Organisation, die Azure Active Directory (Azure AD) B2B-Zusammenarbeitsfunktionen verwendet, um Gastbenutzer aus Partnerorganisationen zu Ihrer Azure AD einzuladen, können Sie diesen B2B-Benutzern jetzt Zugriff auf lokale Apps gewähren. Diese lokalen Apps können samlbasierte Authentifizierung oder integrierte Windows-Authentifizierung (Integrated Windows Authentication, IWA) mit eingeschränkter Kerberos-Delegierung (KCD) verwenden. Weitere Informationen finden Sie unter [Gewähren von B2B-Benutzern in Azure AD Zugriff auf Ihre lokalen Anwendungen](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Erfahren Sie, wie Sie [lokal verwalteten Partnerkonten zugriff auf Cloudressourcen mit Azure AD B2B-Zusammenarbeit gewähren](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).