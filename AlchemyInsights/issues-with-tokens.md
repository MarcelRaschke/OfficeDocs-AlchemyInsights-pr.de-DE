---
title: Probleme mit Token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: c1bd340fff47bbde6457e11e70fed0c983b6256b
ms.sourcegitcommit: f3903d6919d46a31a38edef25d9717a6d005bb15
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2022
ms.locfileid: "65395339"
---
# <a name="issues-with-tokens"></a>Probleme mit Token

Führen Sie die folgenden Schritte durch, um Probleme im Zusammenhang mit Token zu beheben:

1. Sie können die Gültigkeitsdauer für von Microsoft Identity Platform ausgestellte Zugriffs-, ID- oder SAML-Tokens angeben. Sie können die Tokengültigkeitsdauer für alle Apps in Ihrer Organisation festlegen, für eine mehrinstanzfähige (multiorganisatorische) Anwendung oder für einen bestimmten Dienstprinzipal in Ihrer Organisation. Weitere Informationen finden Sie unter [Konfigurierbare Tokengültigkeitsdauer in Microsoft Identity Platform (Vorschau)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Zugriffstoken ermöglichen es Clients, geschützte Web-APIs sicher aufzurufen, und werden von Web-APIs zur Authentifizierung und Autorisierung verwendet. Gemäß der OAuth-Spezifikation sind Zugriffstoken nicht transparente Zeichenfolgen ohne festgelegtes Format. Einige Identitätsanbieter (IDPs) verwenden GUIDs, andere verschlüsselte Blobs. Microsoft Identity Platform verwendet eine Vielzahl von Zugriffstokenformaten, abhängig von der Konfiguration der API, die das Token akzeptiert. Unter [Zugriffstoken von Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint) erfahren Sie, wie Ihre API die Ansprüche in einem Zugriffstoken validieren und verwenden kann.
3. Die Microsoft-Authentifizierungsbibliothek (MSAL) unterstützt mehrere Authentifizierungsabläufe zur Verwendung in verschiedenen Anwendungsszenarien. Weitere Informationen finden Sie unter [Authentifizierungsabläufe](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Die OAuth 2.0-Autorisierungscode-Erteilung kann in Apps verwendet werden, die auf einem Gerät installiert sind, um Zugriff auf geschützte Ressourcen, wie z. B. Web-APIs, zu erhalten. Mit der Microsoft Identity Platform-Implementierung von OAuth 2.0 können Sie Ihren mobilen und Desktop-Apps Anmelde- und API-Zugriff hinzufügen. Weitere Informationen zur direkten Programmierung für das Protokoll in Ihrer Anwendung in einer beliebigen Sprache finden Sie unter [Microsoft Identity Platform und OAuth 2.0 Autorisierungscodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token).
5. OpenID Connect (OIDC) ist ein auf OAuth 2.0 aufbauendes Authentifizierungsprotokoll, das Sie für die sichere Anmeldung eines Benutzers bei einer Anwendung verwenden können. Mit der Microsoft Identity Platform-Endpunktimplementierung von OpenID Connect können Sie Ihren Apps Anmelde- und API-Zugriff hinzufügen. Unter [Microsoft Identity Platform und OpenID Connect-Protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) wird gezeigt, wie dies sprachunabhängig möglich ist, und beschrieben, wie HTTP-Nachrichten gesendet und empfangen werden können, ohne irgendwelche Open-Source-Bibliotheken von Microsoft zu verwenden.
    - Der UserInfo-Endpunkt ist Teil des OIDC-Standards und dient der Rückgabe von Ansprüchen über den Benutzer, der sich authentifiziert hat. Weitere Informationen finden Sie unter [UserInfo-Endpunkt in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Im Beispiel [Aufrufen einer Web-API in einer Web-App unter Verwendung von Azure AD und OpenID Connect](https://github.com/Azure-Samples/active-directory-dotnet-webapp-webapi-openidconnect) wird die Erstellung einer MVC-Webanwendung erläutert, die Azure AD für die Anmeldung über das OpenID Connect-Protokoll verwendet und dann eine Web-API aufruft. Dies erfolgt unter der Identität des angemeldeten Benutzers anhand von Token, die über OAuth 2.0 abgerufen wurden. In diesem Beispiel werden die OpenID Connect ASP .Net OWIN-Middleware und ADAL.Net verwendet.
6. [Konfigurieren einer Anwendung zur Bereitstellung einer Web-API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis): In diesem Schnellstart registrieren Sie eine Web-API bei Microsoft Identity Platform und machen sie für Client-Apps verfügbar, indem Sie einen Beispielbereich hinzufügen. Indem Sie Ihre Web-API registrieren und über Bereiche verfügbar machen, können Sie autorisierten Benutzern und Client-Apps, die auf Ihre API zugreifen, einen berechtigungsbasierten Zugriff auf deren Ressourcen gewähren.
7. In Azure Active Directory B2C (Azure AD B2C) ist der Flow „Anmeldeinformationen des Resourcenbesitzers“ (Resource Owner Password Credentials, ROPC) ein OAuth-Standardauthentifizierungsflow. In diesem Flow tauscht eine Anwendung, die auch als vertrauende Partei bezeichnet wird, gültige Anmeldeinformationen gegen Token aus. Die Anmeldeinformationen umfassen eine Benutzer-ID und ein Kennwort. Die zurückgegebenen Token sind ein ID-Token, ein Zugriffstoken und ein Aktualisierungstoken. Weitere Informationen finden Sie unter [Einrichten eines Flows „Anmeldeinformationen des Resourcenbesitzers“ in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

