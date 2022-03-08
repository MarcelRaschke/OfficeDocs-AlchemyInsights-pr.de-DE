---
title: Probleme mit der Microsoft Graph-API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: 3717720e5945917a362ce843ac642dfe937ab749
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63234699"
---
# <a name="microsoft-graph-api-issues"></a>Probleme mit der Microsoft Graph-API

Dieses Thema kann auch für Entwickler gelten, die weiterhin Azure AD Graph-API verwenden. Es wird jedoch **dringend** empfohlen, Microsoft Graph für alle Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.

**Authentifizierungs- oder Autorisierungsprobleme**

- Wenn Ihre App **keine Token zum** Aufrufen von Microsoft Graph abrufen kann, wählen Sie **Problem beim Abrufen eines Zugriffstokens (Authentifizierung)** Microsoft Graph Kategorie aus, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.
- Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler empfängt**, wählen Sie die Microsoft Graph API-Kategorie "**Zugriff verweigert" aus**, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.

**Ich möchte Microsoft Graph verwenden, aber nicht sicher, wo ich beginnen soll**

- [Übersicht über Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Übersicht über die Identitäts- und Zugriffsverwaltung in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Erste Schritte beim Erstellen von Microsoft Graph-Apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten

**Ich möchte Microsoft Graph verwenden, unterstützt aber die v1.0-Verzeichnis-APIs, die ich benötige?**

Microsoft Graph ist die empfohlene API für Verzeichnis-, Identitäts- und Zugriffsverwaltung. Es gibt jedoch noch einige Lücken zwischen den Möglichkeiten in Azure AD Graph und Microsoft Graph. Lesen Sie die folgenden Artikel, in denen die aktuellsten Unterschiede hervorgehoben werden, um Ihnen bei der Auswahl zu helfen:

- [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodenunterschiede zwischen Azure AD und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Die API, die ich aufrufe, funktioniert nicht – wo kann ich weitere Tests durchführen?**

**Microsoft Graph Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten, und sehen Sie sich auch die **Beispielabfragen** in Microsoft Graph Explorer an.

**Meine App ist zu langsam und wird ebenfalls gedrosselt. Welche Verbesserungen kann ich vornehmen?**

Je nach Szenario stehen Ihnen eine Vielzahl von Optionen zur Verfügung, um ihre Anwendung leistungsstärker und in einigen Fällen weniger anfällig für eine Drosselung durch den Dienst zu machen (wenn Sie zu viele Aufrufe ausführen).

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batchverarbeitungsanforderungen](https://docs.microsoft.com/graph/json-batching)
- [Nachverfolgen von Änderungen über die Delta-Abfrage](https://docs.microsoft.com/graph/delta-query-overview)
- [Benachrichtigung über Änderungen über Webhooks](https://docs.microsoft.com/graph/webhooks)
- [Einschränkungsleitfaden](https://docs.microsoft.com/graph/throttling)

**Wo finde ich weitere Informationen zu Fehlern und bekannten Problemen?**

- [Informationen zur Fehlerantwort von Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Bekannte Probleme in Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Wo kann ich den Status der Dienstverfügbarkeit und -konnektivität überprüfen?**

Die Dienstverfügbarkeit und Konnektivität der zugrunde liegenden Dienste, auf die über Microsoft Graph zugegriffen werden kann, kann sich auf die allgemeine Verfügbarkeit und Leistung von Microsoft Graph auswirken.

- Für Azure Active Directory Dienststatus überprüfen Sie den Status von **Security + Identity-Diensten**, die auf der [Azure-Statusseite](https://azure.microsoft.com/status/) aufgeführt sind.
- For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).

Microsoft Graph Autorisierungsfehler können auf verschiedene Probleme zurückzuführen sein, von denen die meisten einen 401- oder 403-Fehler generieren. Die folgenden Beispiele können zu Autorisierungsfehlern führen:

- Falsche [Flüsse für den Erwerb von Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Schlecht konfigurierte [Berechtigungsumfänge](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Fehlende [Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Ende der Unterstützung für die Azure Active Directory-Authentifizierungsbibliothek (ADAL) und die Azure AD-Graph-API (AAD Graph)***

**Ab dem 30. Juni 2020** werden ADAL und Azure AD Graph keine neuen Features mehr hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.

**Ab dem 30. Juni 2022** beenden wir den Support für ADAL und Azure AD Graph und stellen keinen technischen Support oder sicherheitsrelevante Updates mehr bereit.

Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, *es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt*.

Apps, die Azure AD Graph nach dieser Zeit verwenden, empfangen möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL-Migration**

Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.

Wenn Sie Microsoft-Apps verwenden, wissen Sie, dass Microsoft gerade dabei ist, seine Anwendungen bis zum Ende des Support-Stichtags zu MSAL zu migrieren, um sicherzustellen, dass sie von den laufenden Sicherheits- und Featureverbesserungen von MSAL profitieren.

1. [Häufig gestellte Fragen zu ADAL lesen](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an ISVs oder App-Anbieter zu wenden. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Für Anwendungen, die Azure AD Graph verwenden, befolgen Sie unsere Anleitungen zum [Migrieren Azure AD Graph Apps zu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Unsere Migrationscheckliste stellt einen Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen auch eine Liste aller AAD Graph Nutzung in Ihrem Mandanten bereitstellen.
3. Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. Die [Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) listet die Berechtigungen auf, die den einzelnen Hauptgruppen von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.
