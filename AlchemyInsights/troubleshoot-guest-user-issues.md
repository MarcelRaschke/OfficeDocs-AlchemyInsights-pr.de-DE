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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939378"
---
# <a name="troubleshoot-guest-user-issues"></a>Behandeln von Problemen mit Gastbenutzern

1. Eine Anleitung zum Verwalten des Gastzugriffs auf Anwendungen finden Sie unter [Verwalten des Gastzugriffs mit Azure AD-Zugriffsüberprüfungen.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Fügen Sie Ihrem Verzeichnis im Azure-Portal Gastbenutzer](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)hinzu: In dieser Schnellstartanleitung fügen Sie ihrem Azure AD-Verzeichnis über das Azure-Portal einen neuen Gastbenutzer hinzu, senden eine Einladung und sehen, wie der Einlösungsprozess des Gastbenutzers aussieht.
1. [Hinzufügen eines Gastbenutzers mit PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)In dieser Schnellstartanleitung verwenden Sie den Befehl New-AzureADMSInvitation, um Ihrem Azure-Mandanten einen Gastbenutzer hinzuzufügen.
1. Informationen zum Zuweisen von Benutzern und Gruppen zu Unternehmensanwendungen in Azure Active Directory (Azure AD), entweder im Azure-Portal oder mithilfe von PowerShell, finden Sie unter Verwalten der [Benutzerzuweisung für eine App in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) B2B-Zusammenarbeit funktioniert mit den meisten Apps, die in Azure AD integriert sind. In diesem [Artikel](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)werden Anweisungen zum Konfigurieren einiger beliebter SaaS-Apps für die Verwendung mit Azure AD B2B erläutert.
1. Als Organisation, die die B2B-Zusammenarbeitsfunktionen Azure Active Directory (Azure AD) verwendet, um Gastbenutzer aus Partnerorganisationen zu Azure AD einzuladen, können Sie diesen B2B-Benutzern jetzt Zugriff auf lokale Apps gewähren. Diese lokalen Apps können SAML-basierte Authentifizierung oder integrierte Windows-Authentifizierung (Integrated Windows Authentication, IWA) mit eingeschränkter Kerberos-Delegierung (KCD) verwenden. Weitere Informationen finden Sie unter [Gewähren von B2B-Benutzern in Azure AD Zugriff auf Ihre lokalen Anwendungen.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Erfahren Sie, wie Sie [lokal verwalteten Partnerkonten zugriff auf Cloudressourcen mithilfe der Azure AD B2B-Zusammenarbeit gewähren.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)