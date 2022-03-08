---
title: Authentifizierungsprobleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 33280a944670d33a39b730d00d45e7a708bc2c4a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63094546"
---
# <a name="authentication-issues"></a>Authentifizierungsprobleme

**Suchen Sie nach Informationen zu den AADSTS-Fehlercodes, die vom Azure Active Directory(Azure AD)-Sicherheitstokendienst (STS) zurückgegeben werden?** Informationen zu AADSTS-Fehlern, Korrekturen und einige Vorschläge für die Problemumgehung finden Sie unter [Azure AD-Fehlercodes für Authentifizierung und Autorisierung](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).

Autorisierungsfehler können infolge verschiedener Probleme auftreten, von denen die meisten eine 401- oder 403-Fehlermeldung generieren. Die folgenden Probleme können beispielsweise zu Autorisierungsfehlern führen:

- Falsche [Flüsse für den Erwerb von Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Schlecht konfigurierte [Berechtigungsumfänge](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Fehlende [Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Probieren Sie zur Behebung der häufigsten Fehler die unten angegebenen Schritte aus, die dem angezeigten Fehler am nächsten kommen. Für einen angezeigten Fehler können mehrere Schritte gelten.

**Fehler „401 Unauthorized“: Ist Ihr Token gültig?**

Stellen Sie sicher, dass Ihre Anwendung im Rahmen der Anforderung ein gültiges Zugriffstoken für Microsoft Graph vorweist. Dieser Fehler bedeutet oft, dass das Zugriffstoken im HTTP-Authentifizierungsanforderungs-Header fehlen kann oder dass das Token ungültig oder abgelaufen ist. Wir empfehlen dringend, für den Erwerb von Zugriffstoken die Microsoft Authentication Library (MSAL) zu verwenden. Außerdem kann dieser Fehler auftreten, wenn Sie versuchen, mit einem delegierten Zugriffstoken, das für ein persönliches Microsoft-Konto gewährt wurde, auf eine API zuzugreifen, die nur Organisationskonten (Geschäfts-, Schul- oder Unikonten) unterstützt.

**Fehler „403 Forbidden“: Haben Sie den richtigen Berechtigungssatz ausgewählt?**

Stellen Sie sicher, dass Sie basierend auf den Microsoft Graph-APIs, die von Ihrer Anwendung aufgerufen werden, den richtigen Satz von Berechtigungen angefordert haben. Die empfohlenen Mindestberechtigungen sind in allen Referenzthemen zu Microsoft Graph-API-Methoden enthalten. Darüber hinaus müssen der Anwendung diese Berechtigungen durch einen Benutzer oder einen Administrator gewährt werden. Berechtigungen werden normalerweise über eine Zustimmungsseite oder mithilfe des Anwendungsregistrierungblatts im Azure Portal gewährt. Klicken Sie auf dem Blatt **Einstellungen** für die Anwendung auf **Erforderliche Berechtigungen** und dann auf **Berechtigungen gewähren**. Weitere Informationen finden Sie unter:

- [Microsoft Graph-Berechtigungen](https://docs.microsoft.com/graph/permissions-reference) 
- [Grundlegendes zu Azure AD-Berechtigungen und -Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Fehler „403 Forbidden“: Hat Ihre Anwendung ein Token erworben, das den ausgewählten Berechtigungen entspricht?**

Stellen Sie sicher, dass die Art der angeforderten oder gewährten Berechtigungen mit der Art des Zugriffstokens übereinstimmt, das von Ihrer App erworben wird. Möglicherweise fordern Sie Anwendungsberechtigungen an und gewähren diese, verwenden aber delegierte interaktive Codefluss-Token anstelle von Clientanmeldeinformationsfluss-Token, oder Sie fordern delegierte Berechtigungen an und gewähren diese, verwenden aber Clientanmeldeinformationsfluss-Token anstelle delegierter Codefluss-Token.

Weitere Informationen zum Abrufen von Token finden Sie unter:

- [Zugriff im Namen von Benutzern und delegierte Berechtigungen erhalten](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD Version 2.0 – OAuth 2.0 Autorisierungscode-Fluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Zugriff ohne Benutzer (Daemon-Dienst) und Anwendungsberechtigungen erhalten](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD Version 2.0 – OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Fehler „403 Forbidden“: Passwort zurücksetzen**

Derzeit gibt es keine Anwendungsberechtigungs-Daemon-Dienst-zu-Dienst-Berechtigungen, die das Zurücksetzen von Benutzerkennwörtern zulassen. Diese APIs werden nur unter Verwendung der interaktiven delegierten Codeflüsse mit einem angemeldeten Administrator unterstützt. Weitere Informationen finden Sie unter [Microsoft Graph-Berechtigungen](https://docs.microsoft.com/graph/permissions-reference).

**„403 Forbidden“: Hat der Benutzer Zugriff und ist er lizenziert?**

Bei delegierten Codeflüssen wertet Microsoft Graph aus, ob die Anforderung auf der Grundlage der der Anwendung gewährten Berechtigungen und der Berechtigungen, die der angemeldete Benutzer hat, zulässig ist. Dieser Fehler deutet im Allgemeinen darauf hin, dass der Benutzer nicht genügend Rechte besitzt, die Anforderung auszuführen, **oder** dass der Benutzer nicht für die Daten lizenziert ist, auf die zugegriffen wird. Nur Benutzer mit den erforderlichen Berechtigungen oder Lizenzen können die Anfrage erfolgreich stellen.

**„403 Forbidden“: Haben Sie die richtige Ressourcen-API ausgewählt?**

API-Dienste wie Microsoft Graph überprüfen, ob der *aud*-Anspruch (Zielgruppe) im empfangenen Zugriffstoken mit dem Wert übereinstimmt, den er erwartet. Ist dies nicht der Fall, kommt es zu einem „403 Forbidden“-Fehler. Ein häufiger Fehler, der zu diesem Fehler führt, ist der Versuch, ein für Azure AD-Graph-APIs, Outlook-APIs oder Microsoft Office SharePoint Online-/OneDrive-APIs erworbenes Token zu verwenden, um Microsoft Graph aufzurufen (oder umgekehrt). Stellen Sie sicher, dass die Ressource (oder der Geltungsbereich), für die Ihre Anwendung ein Token erwirbt, mit der API übereinstimmt, die von der Anwendung aufgerufen wird.

**„400 Bad Request“ oder „403 Forbidden“: Entspricht der Benutzer die Richtlinien für den bedingten Zugriff (CA) des Unternehmens?**

Basierend auf den CA-Richtlinien (Conditional Access, bedingter Zugriff) einer Organisation kann ein Benutzer, der über Ihre Anwendung auf Microsoft Graph-Ressourcen zugreift, zur Angabe zusätzlicher Informationen aufgefordert werden, die nicht in dem Zugriffstoken enthalten sind, das Ihre Anwendung ursprünglich erworben hat. In diesem Fall erhält Ihre Anwendung den Fehler **„400“ mit *interaction_required*** beim Erwerb des Zugriffstokens oder einen Fehler **„403“ mit *insufficient_claims*** beim Aufruf von Microsoft Graph. In beiden Fällen enthält die Fehlerantwort zusätzliche Informationen, die dem autorisierten Endpunkt vorgewiesen werden können, um den Benutzer um zusätzliche Informationen zu bitten (wie mehrstufige Authentifizierung oder Geräteregistrierung).

Weitere Informationen zum bedingten Zugriff finden Sie unter:

- [Handhabung von Informationsangabeaufforderungen für bedingten Zugriff mit MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Leitfaden für Entwickler für den bedingten Azure Active Directory-Zugriff](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Ende der Unterstützung für die Azure Active Directory-Authentifizierungsbibliothek (ADAL) und die Azure AD-Graph-API (AAD Graph)***

- Ab dem 30. Juni 2020 werden der Azure Active Directory-Authentifizierungsbibliothek (ADAL) und der Azure AD Graph-API (AAD Graph) keine neuen Features mehr hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.
- Ab dem 30. Juni 2022 werden wir den Support für ADAL und Azure AD Graph beenden und keinen technischen Support oder Sicherheitsupdates mehr dafür bereitstellen.
    - Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt.
    - Apps, die AAD Graph nach diesem Zeitpunkt verwenden, werden keine Antworten mehr vom AAD Graph-Endpunkt erhalten.

**ADAL-Migration**

Es wird ein Update auf die [Microsoft-Authentifizierungsbibliothek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt. Diese Empfehlung steht in Zusammenhang mit der Migration der Anwendungen von Microsoft nach MSAL bis zum Enddatum des Supports. Ziel der Migration von Microsoft-Apps nach MSAL ist es sicherzustellen, dass sie von den laufenden Sicherheits- und Featureverbesserungen von MSAL profitieren.

- [Häufig gestellte Fragen zu ADAL lesen](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Wenn Sie ermitteln müssen, welche Ihrer Apps ADAL verwenden, und dabei Hilfe benötigen, empfehlen wir, den Quellcode Ihrer Apps zu überprüfen und sich ggf. an unabhängige Softwareanbieter (ISVs) oder App-Anbieter zu wenden. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.

**AAD Graph-Migration**

Folgen Sie bei Anwendungen, die AAD Graph verwenden, unseren Anweisungen zum [Migrieren von Azure AD Graph-Apps zu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Unsere Migrationscheckliste stellt einen Ausgangspunkt dar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- In Ihrem Azure-App-Registrierungsportal können Sie sehen, welche Anwendungen AAD Graph verwenden. Es wird empfohlen, sämtlichen Quellcode Ihrer Apps zu überprüfen und sich ggf. mit ISVs oder App-Anbietern in Verbindung zu setzen. Der Microsoft-Support kann Ihnen darüber hinaus Informationen zur gesamten AAD Graph-Nutzung in Ihrem Mandanten bereitstellen.

 










