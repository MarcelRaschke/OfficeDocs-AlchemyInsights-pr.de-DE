---
title: Probleme mit einem Ressourcen- oder Dienstprinzipal
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 51f959d6772071f982502d4143e2f5f3199da382
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66295867"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Probleme mit einem Ressourcen- oder Dienstprinzipal

1. Wenn Sie gerade erst beginnen, beschreiben [Anwendungs- und Dienstprinzipalobjekte in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) die Anwendungsregistrierung, Anwendungsobjekte und Dienstprinzipale in Azure Active Directory: was sie sind, wie sie verwendet werden und wie sie miteinander verbunden sind. Außerdem wird ein Mehrinstanzen-Beispielszenario vorgestellt, um die Beziehung zwischen dem Anwendungsobjekt einer Anwendung und den entsprechenden Dienstprinzipalobjekten zu veranschaulichen.
2. Sie können mehr über die Beziehung zwischen Anwendungen und Dienstprinzipalen erfahren, indem Sie [Anwendungen und Dienstprinzipalobjekte in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) lesen.
3. [Vorgehensweise: Verwenden des Portals zum Erstellen einer Azure AD-Anwendung und eines Dienstprinzipals, die auf Ressourcen zugreifen können](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) , zeigt Ihnen, wie Sie eine neue Azure Active Directory (Azure AD)-Anwendung und einen neuen Dienstprinzipal erstellen, die mit der rollenbasierten Zugriffssteuerung verwendet werden können.
4. Mit der [Dienstprinzipal-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal) können Sie Instanzen von Anwendungen programmgesteuert verwalten und steuern, was eine Anwendung in Ihrem Mandanten tun kann.
5. [Der ressourcentyp servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) listet alle Eigenschaften und Methoden für den servicePrincipal-Ressourcentyp auf.
6. [Ressourcentypunterschiede zwischen Azure AD Graph und Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) hebt Unterschiede zwischen Azure AD Graph- und Microsoft Graph-Ressourcen hervor. Es werden Ressourcen angezeigt, die unterschiedliche Namen haben oder nicht verfügbar sind. außerdem werden Ressourcen hervorgehoben, die in der Betaversion von Microsoft Graph, aber nicht in der Version v1.0 verfügbar sind.

**Probleme mit Gastbenutzern**

- [Schnellstart: Das Hinzufügen von Gastbenutzern zu Ihrem Verzeichnis im Azure-Portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) zeigt Ihnen, wie Sie einen neuen Gastbenutzer über die Azure-Portal zu Ihrem Azure AD-Verzeichnis hinzufügen, eine Einladung senden und sehen, wie der Einlösungsprozess der Einladung des Gastbenutzers aussieht.
- [Lernprogramm: Das Erstellen von Benutzerflüssen in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) zeigt Ihnen, wie Sie einige empfohlene Benutzerabläufe mithilfe der Azure-Portal erstellen. Wenn Sie nach Informationen zum Einrichten eines ROPC-Flusses (Resource Owner Password Credentials, Ressourcenbesitzerkennwortanmeldeinformationen) in Ihrer Anwendung suchen, lesen Sie den Abschnitt "Konfigurieren des Flusses der Kennwortanmeldeinformationen für den Ressourcenbesitzer in Azure AD B2C".
