---
title: Probleme mit einem Ressourcen- oder Dienstprinzipal
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028075"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Probleme mit einem Ressourcen- oder Dienstprinzipal

1. Wenn Sie gerade erst beginnen, beschreiben [Anwendungs- und Dienstprinzipalobjekte in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) die Anwendungsregistrierung, Anwendungsobjekte und Dienstprinzipale in Azure Active Directory: was sie sind, wie sie verwendet werden und wie sie miteinander verbunden sind. Ein mehrinstanzenfähiges Beispielszenario wird auch dargestellt, um die Beziehung zwischen dem Anwendungsobjekt einer Anwendung und den entsprechenden Dienstprinzipalobjekten zu veranschaulichen.
2. Sie können mehr über die Beziehung zwischen Anwendungen und Dienstprinzipalen erfahren, indem Sie [Anwendungen und Dienstprinzipalobjekte in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)lesen.
3. [How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Mit der [Dienstprinzipal-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)können Sie Instanzen von Anwendungen programmgesteuert verwalten und steuern, was eine Anwendung in Ihrem Mandanten tun kann.
5. Der [ressourcentyp servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) listet alle Eigenschaften und Methoden für den ressourcentyp servicePrincipal auf.
6. [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) hebt Unterschiede zwischen Azure AD-Graph und Microsoft Graph-Ressourcen hervor. Es zeigt Ressourcen an, die unterschiedliche Namen haben oder nicht verfügbar sind. Außerdem werden Ressourcen hervorgehoben, die in der Betaversion von Microsoft Graph, jedoch nicht in version 1.0 verfügbar sind.

**Probleme mit Gastbenutzern**

- [Schnellstart: Hinzufügen von Gastbenutzern zu Ihrem Verzeichnis im Azure-Portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) zeigt Ihnen, wie Sie ihrem Azure AD-Verzeichnis über das Azure-Portal einen neuen Gastbenutzer hinzufügen, eine Einladung senden und sehen, wie der Einlösungsprozess des Gastbenutzers aussieht.
- [Lernprogramm: Erstellen von Benutzerabläufen in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) zeigt Ihnen, wie Sie einige empfohlene Benutzerabläufe mithilfe des Azure-Portals erstellen. Informationen zum Einrichten eines ROPC-Flusses (Resource Owner Password Credentials) in Ihrer Anwendung finden Sie unter Konfigurieren des Flusses mit Kennwortanmeldeinformationen für Ressourcenbesitzer in Azure AD B2C.
