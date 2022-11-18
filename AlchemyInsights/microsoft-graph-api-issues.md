---
title: Probleme mit Microsoft Graph-API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: 48ecb7b08513109c684839fcbb79620b37c9de5e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66432643"
---
# <a name="microsoft-graph-api-issues"></a>Probleme mit Microsoft Graph-API

Dieses Thema kann auch für Entwickler gelten, die weiterhin Azure AD Graph-API verwenden. Es wird jedoch **dringend** empfohlen, Microsoft Graph für alle Ihre Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.

**Authentifizierungs- oder Autorisierungsprobleme**

- Wenn Ihre App **keine Token zum** Aufrufen von Microsoft Graph abrufen kann, wählen Sie **"Problem beim Abrufen einer Microsoft Graph-Kategorie für Zugriffstoken (Authentifizierung)** " aus, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.
- Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler empfängt**, wählen Sie die Microsoft Graph-API Kategorie "**Zugriff verweigert" aus**, um spezifischere Hilfe und Support zu diesem Thema zu erhalten.

**Ich möchte Microsoft Graph verwenden, bin mir aber nicht sicher, wo ich anfangen soll**

- [Übersicht über Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Übersicht über die Identitäts- und Zugriffsverwaltung in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Erste Schritte beim Erstellen von Microsoft Graph-Apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph-Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten

**Ich möchte Microsoft Graph verwenden, unterstützt aber die v1.0-Verzeichnis-APIs, die ich benötige?**

Microsoft Graph ist die empfohlene API für die Verzeichnis-, Identitäts- und Zugriffsverwaltung. Es gibt jedoch noch ein paar Lücken zwischen dem, was in Azure AD Graph und Microsoft Graph möglich ist. Lesen Sie die folgenden Artikel, in denen die aktuellsten Unterschiede hervorgehoben werden, die Sie bei Ihrer Auswahl unterstützen können:

- [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodenunterschiede zwischen Azure AD und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Die API, die ich aufrufe, funktioniert nicht – wo kann ich weitere Tests durchführen?**

**Microsoft Graph-Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten, und schauen Sie sich auch die **Beispielabfragen** im Microsoft Graph-Explorer an.

**Meine App ist zu langsam und wird auch gedrosselt. Welche Verbesserungen kann ich vornehmen?**

Je nach Szenario stehen Ihnen eine Vielzahl von Optionen zur Verfügung, um die Leistung Ihrer Anwendung zu verbessern und in einigen Fällen weniger anfällig für eine Drosselung durch den Dienst zu sein (wenn Sie zu viele Aufrufe tätigen).

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Batchverarbeitungsanforderungen](https://docs.microsoft.com/graph/json-batching)
- [Nachverfolgen von Änderungen über delta-Abfrage](https://docs.microsoft.com/graph/delta-query-overview)
- [Erhalten von Benachrichtigungen über Änderungen über Webhooks](https://docs.microsoft.com/graph/webhooks)
- [Drosselungsleitfaden](https://docs.microsoft.com/graph/throttling)

**Wo finde ich weitere Informationen zu Fehlern und bekannten Problemen?**

- [Microsoft Graph-Fehlerantwortinformationen](https://docs.microsoft.com/graph/errors)
- [Bekannte Probleme in Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Wo kann ich den Status der Dienstverfügbarkeit und -konnektivität überprüfen?**

Die Dienstverfügbarkeit und -konnektivität der zugrunde liegenden Dienste, auf die über Microsoft Graph zugegriffen werden kann, kann sich auf die allgemeine Verfügbarkeit und Leistung von Microsoft Graph auswirken.

- Überprüfen Sie für den Azure Active Directory-Dienststatus den Status von **Sicherheits- und Identitätsdiensten** , die auf der [Azure-Statusseite](https://azure.microsoft.com/status/) aufgeführt sind.
- Überprüfen Sie für Office-Dienste, die zu Microsoft Graph beitragen, den Status der Dienste, die im [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth) aufgeführt sind.

Microsoft Graph-Autorisierungsfehler können auf verschiedene Probleme zurückzuführen sein, von denen die meisten einen Fehler 401 oder 403 generieren. Die folgenden Beispiele können zu Autorisierungsfehlern führen:

- Falsche [Flüsse für den Erwerb von Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Schlecht konfigurierte [Berechtigungsumfänge](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Fehlende [Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Ende der Unterstützung für die Azure Active Directory-Authentifizierungsbibliothek (ADAL) und die Azure AD-Graph-API (AAD Graph)***

**Ab dem 30. Juni 2020** werden wir ADAL und Azure AD Graph keine neuen Features mehr hinzufügen. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.

**Ab dem 30. Juni 2022** beenden wir den Support für ADAL und Azure AD Graph und stellen keine technischen Support- oder Sicherheitsupdates mehr bereit.

Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, *es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt*.

Apps, die Azure AD Graph nach dieser Zeit verwenden, empfangen möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL-Migration**

Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.

Wenn Sie Microsoft-Apps verwenden, wissen Sie, dass Microsoft gerade dabei ist, seine Anwendungen bis zum Ende des Support-Stichtags zu MSAL zu migrieren, um sicherzustellen, dass sie von den kontinuierlichen Sicherheits- und Featureverbesserungen von MSAL profitieren.

1. [Häufig gestellte Fragen zu ADAL lesen](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden, empfehlen wir Ihnen, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an alle ISVs oder App-Anbieter zu wenden. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Befolgen Sie für Anwendungen, die Azure AD Graph verwenden, unsere Anleitung zum [Migrieren von Azure AD Graph-Apps zu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Unsere Migrationscheckliste stellt einen Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen auch eine Liste aller AAD Graph-Nutzungen in Ihrem Mandanten bereitstellen.
3. Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. Die [Microsoft Graph-Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) listet die Berechtigungen auf, die den einzelnen Hauptsätzen von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.
