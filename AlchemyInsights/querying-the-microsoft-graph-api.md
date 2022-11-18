---
title: Abfragen der Microsoft Graph-API
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
- "7846"
ms.openlocfilehash: add6fd7971892bac387d68cab7cd4e4dac6115d0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66400143"
---
# <a name="querying-the-microsoft-graph-api"></a>Abfragen der Microsoft Graph-API

Dieses Thema kann auch für Entwickler gelten, die weiterhin Azure AD Graph-API verwenden. Es wird jedoch **dringend** empfohlen, Microsoft Graph für alle Ihre Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.

**Authentifizierungs- oder Autorisierungsprobleme**

- Wenn Ihre App **keine Token zum** Aufrufen von Microsoft Graph abrufen kann, wählen Sie **"Problem beim Abrufen einer Microsoft Graph-Kategorie für Zugriffstoken (Authentifizierung)** " aus, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.
- Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler empfängt**, wählen Sie die Microsoft Graph-API Kategorie "**Zugriff verweigert" aus**, um spezifischere Hilfe und Support zu diesem Thema zu erhalten.

**Ich möchte Microsoft Graph verwenden, bin mir aber nicht sicher, wo ich anfangen soll**

Weitere Informationen zu Microsoft Graph finden Sie unter:

- [Übersicht über Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Übersicht über die Identitäts- und Zugriffsverwaltung in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Erste Schritte beim Erstellen von Microsoft Graph-Apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph-Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten

**Ich möchte Microsoft Graph verwenden, unterstützt aber die v1.0-Verzeichnis-APIs, die ich benötige?**

Microsoft Graph ist die empfohlene API für die Verzeichnis-, Identitäts- und Zugriffsverwaltung. Es gibt jedoch noch ein paar Lücken zwischen dem, was in Azure AD Graph und Microsoft Graph möglich ist. Lesen Sie die folgenden Artikel, in denen die aktuellsten Unterschiede hervorgehoben werden, die Sie bei Ihrer Auswahl unterstützen können:

- [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodenunterschiede zwischen Azure AD und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Wenn ich das *Benutzerobjekt* abfrage, fehlen viele seiner Eigenschaften**

`GET https://graph.microsoft.com/v1.0/users` gibt nur 11 Eigenschaften zurück, da Microsoft Graph automatisch einen Standardsatz von *Benutzereigenschaften* auswählt, die zurückgegeben werden sollen. Wenn Sie andere *Benutzereigenschaften* benötigen, verwenden Sie $select, um die Eigenschaften zu wählen, die Ihre Anwendung benötigt. Probieren Sie es zuerst im **Microsoft Graph-Explorer** aus.

**Einige Benutzereigenschaftswerte sind *null* , obwohl ich weiß, dass sie festgelegt sind**

Die wahrscheinlichste Erklärung ist, dass der Anwendung die Berechtigung *User.ReadBasic.All* erteilt wurde. Auf diese Weise kann die Anwendung einen begrenzten Satz von Benutzereigenschaften lesen, wodurch alle anderen Eigenschaften als NULL zurückgegeben werden, auch wenn sie zuvor festgelegt wurden. Versuchen Sie stattdessen, der Anwendung *User.Read.All* die Berechtigung zu erteilen.

Weitere Informationen finden Sie unter [Microsoft Graph-Benutzerberechtigungen](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Ich habe Probleme mit der Verwendung von OData-Abfrageparametern zum Filtern von Daten in meinen Anforderungen**

Während Microsoft Graph einen breiten Bereich der OData-Abfrageparameter unterstützt, werden viele dieser Parameter von Verzeichnisdiensten (Ressourcen, die von *directoryObject* erben) in Microsoft Graph nicht vollständig unterstützt. Die gleichen Einschränkungen, die in Azure AD Graph vorhanden waren, bleiben größtenteils in Microsoft Graph bestehen:

1. **Nicht unterstützt**: $count, $search und $filter für *NULL-* oder *null-Werte*
2. **Nicht unterstützt**: $filter für bestimmte Eigenschaften (siehe Ressourcenthemen, welche Eigenschaften filterbar sind)
3. **Nicht unterstützt**: Gleichzeitiges Paging, Filtern und Sortieren
4. **Nicht unterstützt**: Filtern nach einer Beziehung. Beispiel: Suchen Sie alle Mitglieder der Engineering-Gruppe, die sich in Großbritannien befinden.
5. **Teilweise Unterstützung**: $orderby für *Benutzer* (nur displayName und userPrincipalName) und *Gruppe*
6. **Partielle Unterstützung**: $filter (unterstützt nur *eq*, *startswith* *oder* *und, und*, und *beschränkte)* Unterstützung, $expand (das Erweitern der Beziehungen eines einzelnen Objekts gibt alle Beziehungen zurück, aber das Erweitern einer Auflistung von Objektbeziehungen ist begrenzt)

Weitere Informationen finden [Sie unter Anpassen von Antworten mit Abfrageparametern](https://docs.microsoft.com/graph/query-parameters).

**Die API, die ich aufrufe, funktioniert nicht – wo kann ich weitere Tests durchführen?**

**Microsoft Graph-Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten, und schauen Sie sich auch die **Beispielabfragen** im Microsoft Graph-Explorer an.

**Wenn ich datenabfrage, scheint es, als erhalte ich einen unvollständigen Datensatz zurück**

Wenn Sie eine Sammlung abfragen (z. B. *Benutzer*), verwendet Microsoft Graph serverseitige Seitenbeschränkungen, sodass Die Ergebnisse immer mit einer Standardseitengröße zurückgegeben werden. Ihre App sollte immer erwarten, dass sie sammlungen durchläuft, die vom Dienst zurückgegeben werden.

Weitere Informationen finden Sie unter:

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging der Microsoft Graph-Daten in Ihrer App](https://docs.microsoft.com/graph/paging)

**Meine App ist zu langsam und wird auch gedrosselt. Welche Verbesserungen kann ich vornehmen?**

Je nach Szenario stehen Ihnen verschiedene Optionen zur Verfügung, um die Leistung Ihrer Anwendung zu verbessern und in einigen Fällen weniger anfällig für eine Drosselung durch den Dienst zu sein (wenn Sie zu viele Anrufe tätigen).

Weitere Informationen finden Sie unter:

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
