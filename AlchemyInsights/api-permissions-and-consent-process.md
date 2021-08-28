---
title: API-Berechtigungen und Zustimmungsprozess
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932060"
---
# <a name="api-permissions-and-consent-process"></a>API-Berechtigungen und Zustimmungsprozess

Damit Ihre App auf Daten in Microsoft Graph zugreifen kann, muss der Benutzer oder Administrator ihr die korrekten Berechtigungen über einen Einwilligungsvorgang erteilen. [Microsoft Graph Berechtigungsreferenz](https://docs.microsoft.com/graph/permissions-reference) listet die Berechtigungen auf, die den einzelnen Hauptgruppen von Microsoft Graph-APIs zugeordnet sind. Es enthält auch Anleitungen zur Verwendung der Berechtigungen.

**Einrichten oder Aktualisieren des Dienstprinzipals**

- [Serviceprincipal erstellen](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – In diesem Artikel wird gezeigt, wie Sie ein neues servicePrincipal-Objekt erstellen.
- [Erstellen Sie eine Azure AD-App & Dienstprinzipal im Portal.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) In diesem Artikel wird gezeigt, wie Sie eine neue Azure Active Directory (Azure AD)-Anwendung und einen Dienstprinzipal erstellen, die mit der rollenbasierten Zugriffssteuerung verwendet werden können.
- [Apps & Dienstprinzipale in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – In diesem Artikel werden anwendungsregistrierung, Anwendungsobjekte und Dienstprinzipale in Azure Active Directory beschrieben: was sie sind, wie sie verwendet werden und wie sie miteinander verbunden sind.

**Hinzufügen oder Aktualisieren der App-Registrierung und Erteilen der Administratorzustimmung**

- [Erstellen einer App-Registrierung](https://docs.microsoft.com/graph/api/application-post-applications) – In diesem Artikel wird gezeigt, wie Sie ein neues Anwendungsobjekt erstellen.
- [Aktualisieren einer App-Registrierung – API-Berechtigungen](https://docs.microsoft.com/graph/api/application-update) – In diesem Artikel wird gezeigt, wie Sie die Eigenschaften eines Anwendungsobjekts aktualisieren.
- [Bereitstellen der Administratorzustimmung](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – Für die Administratorzustimmung und -zustimmung im Allgemeinen ist es erforderlich, dass ein Administrator die Zustimmung explizit erteilt.
- [RBAC (Beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Rollenverwaltungscontainer für einheitliche Rollendefinitionen und Rollenzuweisungen für Microsoft 365 RBAC-Anbieter, die mehrere Prinzipale und mehrere Bereiche in einer einzelnen Rollenzuweisung unterstützen. Dies unterscheidet sich vom *rbacApplication-Ressourcentyp.* Microsoft Intune ist ein Beispiel für einen solchen RBAC-Anbieter. Eine Rollenzuweisung in Intune kann ein Array von Prinzipalen und ein Array von Bereichsgruppen enthalten. **Dies ist in der Betaversion, d. h., sie befindet sich noch in der Entwicklung und wird nicht für die Verwendung in der Produktion empfohlen.**
