---
title: Probleme bei der Entwicklung von Anwendungen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004342"
- "7754"
ms.date: 01/25/2021
ms.openlocfilehash: 91bed409b771101420d848667fd9f7e6a8d3ff3c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66404824"
---
# <a name="issues-developing-applications"></a>Probleme bei der Entwicklung von Anwendungen

Informationen zur Behebung der häufigsten Probleme beim Entwickeln von Azure Active Directory (AD)-Apps finden Sie in den folgenden Artikeln:

- [Es gibt Probleme beim Anmelden bei Anwendungen nur mit dem Chrome-Browser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ich weiß nicht, wie ich die Standardeinstellungen für die Gültigkeitsdauer von Token für meine Anwendung ändern kann](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Mir ist unklar, wie die Zustimmung für Anwendungen funktioniert](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ich weiß nicht, wie Berechtigungen für meine Anwendung erteilt werden](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Mir ist der Unterschied zwischen delegierten und Anwendungsberechtigungen nicht klar](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Ende der Unterstützung für die Azure Active Directory-Authentifizierungsbibliothek (ADAL) und die Azure AD-Graph-API (AAD Graph)***

- Ab dem 30. Juni 2020 werden der Azure Active Directory-Authentifizierungsbibliothek (ADAL) und der Azure AD Graph-API (AAD Graph) keine neuen Features mehr hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.

- Ab dem 30. Juni 2022 werden wir den Support für ADAL und Azure AD Graph beenden und keinen technischen Support oder Sicherheitsupdates mehr dafür bereitstellen. Dies wird folgende Auswirkungen haben:

    - Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt.

    - Apps, die AAD Graph nach diesem Zeitpunkt verwenden, werden keine Antworten mehr vom AAD Graph-Endpunkt erhalten.

**ADAL-Migration**

Wenn Sie Microsoft-Apps verwenden, wird ein Update auf die Microsoft-Authentifizierungsbibliothek (MSAL) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt. Diese Empfehlung steht in Zusammenhang mit dem Beginn der Migration der eigenen Anwendungen durch Microsoft nach MSAL bis zum Enddatum des Supports. 

Durch die Migration der eigenen Apps durch Microsoft zu MSAL wird sichergestellt, dass sie von den ständigen Sicherheits- und Featureverbesserungen für MSAL profitieren.

1. [Häufig gestellte Fragen zu ADAL lesen](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Wenn Sie ermitteln müssen, welche Ihrer Apps ADAL verwenden, und dabei Hilfe benötigen, empfehlen wir, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an unabhängige Softwareanbieter (ISVs) oder App-Anbieter zu wenden. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Folgen Sie bei Anwendungen, die AAD Graph verwenden, unseren Anweisungen zum Migrieren von Azure AD Graph-Apps zu Microsoft Graph:

1. [Unsere Migrationscheckliste stellt einen guten Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, den Quellcode all Ihrer Apps zu überprüfen, und sich ggf. mit unabhängigen Softwareanbietern (ISVs) oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen darüber hinaus Informationen zur AAD Graph-Nutzung in Ihrem Mandanten bereitstellen.







