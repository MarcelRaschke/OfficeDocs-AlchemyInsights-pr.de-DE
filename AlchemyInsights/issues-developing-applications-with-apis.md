---
title: Probleme beim Entwickeln von Anwendungen mit APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013459"
---
# <a name="issues-developing-applications-with-apis"></a>Probleme beim Entwickeln von Anwendungen mit APIs

Wenn Sie mit der Verwendung der Azure Active Directory Graph-API beginnen möchten, lesen Sie die [Schnellstartanleitung zur Azure AD-Graph-API,](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) oder sehen Sie sich die [api-Referenzdokumentation für interaktive Azure AD-Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)an.

**Ende der Unterstützung für Azure Active Directory Authentication Library (ADAL) und azure AD Graph API (AAD Graph)**

**Ab dem 30. Juni 2020** werden keine neuen Features mehr zu ADAL und Azure AD Graph hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.

**Ab dem 30. Juni 2022** beenden wir den Support für ADAL und Azure AD Graph und stellen keinen technischen Support oder sicherheitsrelevante Updates mehr bereit.

Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt.

Apps, die Azure AD Graph nach dieser Zeit verwenden, empfangen möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL-Migration**

Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.

Wenn Sie Microsoft-Apps verwenden, wissen Sie, dass Microsoft gerade dabei ist, seine Anwendungen bis zum Ende des Support-Stichtags zu MSAL zu migrieren, um sicherzustellen, dass sie von den laufenden Sicherheits- und Featureverbesserungen von MSAL profitieren.

1. [Lesen Sie hierzu die häufig gestellten Fragen zu ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an ISVs oder App-Anbieter zu wenden. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Für Anwendungen, die Azure AD Graph verwenden, befolgen Sie unsere Anleitungen zum Migrieren von [Azure AD Graph-Apps zu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Unsere Migrationscheckliste stellt einen guten Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen auch eine Liste aller AAD-Graph Nutzung in Ihrem Mandanten bereitstellen.
1. Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. In [der Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) für Microsoft Graph sind die Berechtigungen aufgeführt, die den einzelnen Hauptgruppen von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.
