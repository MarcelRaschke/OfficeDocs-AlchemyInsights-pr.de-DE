---
title: Probleme mit Authentifizierungsbibliotheken
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028003"
---
# <a name="issues-with-authentication-libraries"></a>Probleme mit Authentifizierungsbibliotheken

1. [Microsoft Identity Platform Authentifizierungsbibliotheken listet](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) von Microsoft unterstützte und kompatible Client- und Middlewarebibliotheken auf.
2. Die Microsoft-Authentifizierungsbibliothek (MSAL) unterstützt mehrere [Authentifizierungsflüsse](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) für die Verwendung in verschiedenen Anwendungsszenarien.
3. Um Token zu authentifizieren und zu erwerben, initialisieren Sie eine neue öffentliche oder vertrauliche Clientanwendung in Ihrem Code. Sie können mehrere Konfigurationsoptionen festlegen, wenn Sie die Client-App in der Microsoft-Authentifizierungsbibliothek (MSAL) initialisieren. Weitere Informationen finden Sie unter ["Anwendungskonfigurationsoptionen".](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Ende der Unterstützung für Azure Active Directory Authentication Library (ADAL) und azure AD Graph API (AAD Graph)**

**Ab dem 30. Juni 2020** werden keine neuen Features mehr zu ADAL und Azure AD Graph hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.

**Ab dem 30. Juni 2022** beenden wir den Support für ADAL und Azure AD Graph und stellen keinen technischen Support oder sicherheitsrelevante Updates mehr bereit.

Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, *es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt*.

Apps, die Azure AD Graph nach dieser Zeit verwenden, empfangen möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL-Migration**

Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.

Wenn Sie Microsoft-Apps verwenden, wissen Sie, dass Microsoft gerade dabei ist, seine Anwendungen bis zum Ende des Support-Stichtags zu MSAL zu migrieren, um sicherzustellen, dass sie von den laufenden Sicherheits- und Featureverbesserungen von MSAL profitieren.

Weitere Informationen finden Sie unter:

1. [Häufig gestellte Fragen zu ADAL lesen](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an ISVs oder App-Anbieter zu wenden. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Für Anwendungen, die Azure AD Graph verwenden, befolgen Sie unsere Anleitungen zum [Migrieren von Azure AD Graph-Apps zu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Unsere Migrationscheckliste bietet einen Einstiegspunkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen auch eine Liste aller AAD-Graph Nutzung in Ihrem Mandanten bereitstellen.
3. Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. In [der Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) für Microsoft Graph sind die Berechtigungen aufgeführt, die den einzelnen Hauptgruppen von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.
