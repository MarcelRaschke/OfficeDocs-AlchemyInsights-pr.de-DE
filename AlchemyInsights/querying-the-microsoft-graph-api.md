---
title: Abfragen der Microsoft Graph-API
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
- "7846"
ms.openlocfilehash: da7eb05e21c8556d8a52b8894f1e1ca2c568a394
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63125921"
---
# <a name="querying-the-microsoft-graph-api"></a>Abfragen der Microsoft Graph-API

Dieses Thema kann auch für Entwickler gelten, die weiterhin Azure AD Graph-API verwenden. Es wird jedoch **dringend** empfohlen, Microsoft Graph für alle Verzeichnis-, Identitäts- und Zugriffsverwaltungsszenarien zu verwenden.

**Authentifizierungs- oder Autorisierungsprobleme**

- Wenn Ihre App **keine Token zum** Aufrufen von Microsoft Graph abrufen kann, wählen Sie **Problem beim Abrufen eines Zugriffstokens (Authentifizierung)** Microsoft Graph Kategorie aus, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.
- Wenn Ihre App beim Aufrufen von Microsoft Graph **401- oder 403-Autorisierungsfehler empfängt**, wählen Sie die Microsoft Graph API-Kategorie "**Zugriff verweigert" aus**, um spezifischere Hilfe und Unterstützung zu diesem Thema zu erhalten.

**Ich möchte Microsoft Graph verwenden, aber nicht sicher, wo ich beginnen soll**

Weitere Informationen zu Microsoft Graph finden Sie unter:

- [Übersicht über Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Übersicht über die Identitäts- und Zugriffsverwaltung in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Erste Schritte beim Erstellen von Microsoft Graph-Apps](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Testen von Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten

**Ich möchte Microsoft Graph verwenden, unterstützt aber die v1.0-Verzeichnis-APIs, die ich benötige?**

Microsoft Graph ist die empfohlene API für Verzeichnis-, Identitäts- und Zugriffsverwaltung. Es gibt jedoch noch einige Lücken zwischen den Möglichkeiten in Azure AD Graph und Microsoft Graph. Lesen Sie die folgenden Artikel, in denen die aktuellsten Unterschiede hervorgehoben werden, um Ihnen bei der Auswahl zu helfen:

- [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Eigenschaftsunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Methodenunterschiede zwischen Azure AD und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Wenn ich das *Benutzerobjekt* abfrage, fehlen viele seiner Eigenschaften**

`GET https://graph.microsoft.com/v1.0/users`gibt nur 11 Eigenschaften zurück, da Microsoft Graph automatisch einen Standardsatz von *Benutzereigenschaften* auswählt, der zurückgegeben werden soll. Wenn Sie andere *Benutzereigenschaften* benötigen, verwenden Sie $select, um die Eigenschaften zu wählen, die Ihre Anwendung benötigt. Probieren Sie es zuerst in **Microsoft Graph Explorer** aus.

**Einige Benutzereigenschaftswerte sind *null* , obwohl ich weiß, dass sie festgelegt sind.**

Die wahrscheinlichste Erklärung ist, dass der Anwendung die Berechtigung *User.ReadBasic.All* gewährt wurde. Dadurch kann die Anwendung einen begrenzten Satz von Benutzereigenschaften lesen und alle anderen Eigenschaften als NULL zurückgeben, auch wenn sie zuvor festgelegt wurden. Versuchen Sie stattdessen, der Anwendung " *User.Read.All"* die Berechtigung zu erteilen.

Weitere Informationen finden Sie unter [Microsoft Graph Benutzerberechtigungen](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Ich habe Probleme mit der Verwendung von OData-Abfrageparametern zum Filtern von Daten in meinen Anforderungen**

Während Microsoft Graph eine Vielzahl von OData-Abfrageparametern unterstützt, werden viele dieser Parameter von Verzeichnisdiensten (Ressourcen, die von *directoryObject* erben) in Microsoft Graph nicht vollständig unterstützt. Die gleichen Einschränkungen, die in Azure AD Graph vorhanden waren, bleiben größtenteils in Microsoft Graph bestehen:

1. **Nicht unterstützt**: $count, $search und $filter für *NULL-Werte* oder *nicht NULL-Werte*
2. **Nicht unterstützt**: $filter zu bestimmten Eigenschaften (siehe Ressourcenthemen, in denen Eigenschaften gefiltert werden können)
3. **Nicht unterstützt**: Gleichzeitiges Paging, Filtern und Sortieren
4. **Nicht unterstützt**: Filtern nach einer Beziehung. Suchen Sie beispielsweise alle Mitglieder der Engineering-Gruppe, die sich in Großbritannien befinden.
5. **Teilweise Unterstützung**: $orderby für *Benutzer* (nur displayName und userPrincipalName) und *Gruppe*
6. **Partielle Unterstützung**: $filter (unterstützt nur *eq*, *startswith* *oder**, and, and* limited *any*) Unterstützung, $expand (das Erweitern der Beziehungen eines einzelnen Objekts gibt alle Beziehungen zurück, aber das Erweitern einer Auflistung von Objektbeziehungen ist begrenzt)

Weitere Informationen finden Sie unter [Anpassen von Antworten mit Abfrageparametern](https://docs.microsoft.com/graph/query-parameters).

**Die API, die ich aufrufe, funktioniert nicht – wo kann ich weitere Tests durchführen?**

**Microsoft Graph Explorer** – Testen Sie Microsoft Graph-APIs in Ihrem Mandanten oder einem Demomandanten, und sehen Sie sich auch die **Beispielabfragen** in Microsoft Graph Explorer an.

**Wenn ich Daten abfrage, sieht es so aus, als erhalte ich einen unvollständigen Datensatz zurück**

Wenn Sie eine Sammlung (z. B. *Benutzer*) abfragen, verwendet Microsoft Graph serverseitige Seitenbeschränkungen, sodass Ergebnisse immer mit einer Standardseitengröße zurückgegeben werden. Ihre App sollte immer davon ausgehen, dass Sammlungen durchblättern, die vom Dienst zurückgegeben werden.

Weitere Informationen finden Sie unter:

- [Bewährte Methoden für Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging der Microsoft Graph-Daten in Ihrer App](https://docs.microsoft.com/graph/paging)

**Meine App ist zu langsam und wird ebenfalls gedrosselt. Welche Verbesserungen kann ich vornehmen?**

Je nach Szenario stehen Ihnen verschiedene Optionen zur Verfügung, um ihre Anwendung leistungsstärker und in einigen Fällen weniger anfällig für eine Drosselung durch den Dienst zu machen (wenn Sie zu viele Aufrufe ausführen).

Weitere Informationen finden Sie unter:

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
