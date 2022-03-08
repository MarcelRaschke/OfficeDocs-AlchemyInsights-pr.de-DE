---
title: Probleme mit Links und URLs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: dbfd815c113f1826dba8879dbdca8f9733934f95
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63256114"
---
# <a name="issues-with-links-and-urls"></a>Probleme mit Links und URLs

Umleitungs-URI/Antwort-URLs (beide Ausdrücke sind austauschbar) sind die URLs, die von Microsoft Identity Platform verwendet werden, um von der App angeforderte Token zurückzugeben. Informationen zu diesen URLs finden Sie in den folgenden Artikeln:

- [Authentifizierungsabläufe und Anwendungsszenarien](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Informationen zu den Umleitungs-URIs auf der **App-Registrierungsseite** für jedes Szenario.
- [Umleitungs-URIs/Antwort-URL – Einschränkungen und Begrenzungen](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ich weiß nicht, wie der richtige Umleitungs-URI/die richtige Antwort-URL für meine App registriert wird**

Wenn bei der Anmeldung bei der App, die Sie entwickeln, im Anmeldedialogfeld **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application (Die in der Anforderung angegebene Antwort-URL stimmt nicht mit den für diese App konfigurierten Antwort-URLs überein)\<your app ID\>** angezeigt wird, müssen Sie Ihrer Anwendungsregistrierung den Umleitungs-URI hinzufügen, den Ihr Code in der Tokenanforderung an die Microsoft-Identitätsplattform verwendet hat.

Wechseln Sie zum Hinzufügen einer Antwort-URL im Azure-Portal auf der **Anwendungsregistrierungsseite** zur Registerkarte **Authentifizierung**, und fügen Sie im Abschnitt **Umleitungs-URIs** einen Eintrag hinzu. Der Wert, den Sie eingeben müssen, hängt von der Art der von Ihnen erstellten Anwendung ab, wie nachstehend beschrieben:

- Bei Anwendungen mit nur einer Seite und Web-Apps ist die Antwort-URL eine URL in Ihrer Anwendung. Siehe [Registrieren von Einzelseiten-Apps ](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) oder [Registrieren einer Web-App über das Azure-Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal).
- Bei Desktop-Apps hängt der auszuwählende Wert von Folgendem ab:
    - der Plattform (MacOS unterscheidet sich von Windows oder Linux)
    - der Art und Weise, wie das Token erworben wird (interaktiv, via Gerätecodefluss, integrierter Windows-Authentifizierung [IWA] oder Benutzername/Kennwort).
    Weitere Informationen finden Sie unter [Desktop-Apps: App-Registrierung – Umleitungs-URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris).
- Bei mobilen Anwendungen hängt der Umleitungs-URI von Folgendem ab:
    - der Plattform (iOS/Android/UWP)
    - die Informationen, die zum Erstellen Ihrer App verwendet werden, z. B. die Bundle-ID in iOS, und der Paketname und der Signatur-Hash unter Android. Die Azure-Portal-App-Registrierung hilft Ihnen. Weitere Informationen finden Sie unter [Plattformkonfiguration und Umleitungs-URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Hinweis**: Web-APIs und einige der Arten des Abrufens von Token im Hintergrund (IWA und Benutzername/Kennwort) erfordern keinen Umleitungs-URI.

**Ich habe meine Webanwendung bereitgestellt, und wenn ich sie teste, wird die Meldung angzeigt, dass die Antwort-URL nicht übereinstimmend ist.**

Fügen Sie Umleitungs-URIs für alle Orte hinzu, an denen Sie die Webanwendung bereitstellen. Weitere Informationen finden Sie unter [Registrieren einer Web-App über das Azure-Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Hinweis**: Fügen Sie einen Umleitungs-URI für einen Ort unmittelbar nach der Bereitstellung der Anwendung an diesem Ort hinzu.

**Ich kann nicht genügend Antwort-URLs registrieren.**

Sie sind ein unabhängiger Softwarehersteller (ISV) und es gibt eine oder mehrere Umleitungs-URIs für jeden Kunden. Sie möchten von ADAL/Azure AD v1.0 zu MSAL/der Microsoft Identity Platform migrieren, und Sie haben die [maximale Anzahl von Umleitungs-URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) erreicht. Um dieses Problem zu beheben, [fügen Sie Umleitungs-URIs zu den Dienstprinzipalen hinzu](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), die dem jeweiligen Kunden entsprechen.
