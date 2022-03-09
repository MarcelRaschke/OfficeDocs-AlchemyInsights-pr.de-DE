---
title: API-Berechtigungen und Zustimmungsprozess
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: cebc8ff75fc92eded471d38378b38d22aa31f8db
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63308633"
---
# <a name="api-permissions-and-consent-process"></a>API-Berechtigungen und Zustimmungsprozess

Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. [Microsoft Graph Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) listet die Berechtigungen auf, die den einzelnen Hauptgruppen von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.

**Einrichten oder Aktualisieren des Dienstprinzipals**

- [Serviceprincipal erstellen](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – In diesem Artikel wird gezeigt, wie Sie ein neues servicePrincipal-Objekt erstellen.
- [Erstellen Sie eine Azure AD App & Dienstprinzipals im Portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal). In diesem Artikel wird gezeigt, wie Sie eine neue Azure Active Directory anwendung (Azure AD) und einen Dienstprinzipal erstellen, die mit der rollenbasierten Zugriffssteuerung verwendet werden können.
- [Apps & Dienstprinzipale in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Dieser Artikel beschreibt die Anwendungsregistrierung, Anwendungsobjekte und Dienstprinzipale in Azure Active Directory: was sie sind, wie sie verwendet werden und wie sie miteinander verbunden sind.

**Hinzufügen oder Aktualisieren der App-Registrierung und Erteilen der Administratorzustimmung**

- [Erstellen einer App-Registrierung](https://docs.microsoft.com/graph/api/application-post-applications) – In diesem Artikel erfahren Sie, wie Sie ein neues Anwendungsobjekt erstellen.
- [Aktualisieren einer App-Registrierung – API-Berechtigungen](https://docs.microsoft.com/graph/api/application-update) – In diesem Artikel wird gezeigt, wie Sie die Eigenschaften eines Anwendungsobjekts aktualisieren.
- [Bereitstellen der Administratorzustimmung](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – Für die Administratorzustimmung und -zustimmung im Allgemeinen ist es erforderlich, dass ein Administrator die Zustimmung explizit erteilt.
- [RBAC (Beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Rollenverwaltungscontainer für einheitliche Rollendefinitionen und Rollenzuweisungen für Microsoft 365 RBAC-Anbieter, die mehrere Prinzipale und mehrere Bereiche in einer einzelnen Rollenzuweisung unterstützen. Dies unterscheidet sich vom *rbacApplication-Ressourcentyp* . Microsoft Intune ist ein Beispiel für einen solchen RBAC-Anbieter. Eine Rollenzuweisung in Intune kann ein Array von Prinzipalen und ein Array von Bereichsgruppen enthalten. **Dies ist in der Betaversion, d. h., sie befindet sich noch in der Entwicklung und wird nicht für die Verwendung in der Produktion empfohlen.**
