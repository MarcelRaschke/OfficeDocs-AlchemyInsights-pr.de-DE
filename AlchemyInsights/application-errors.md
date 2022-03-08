---
title: Anwendungsfehler
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: d565a5892651af89083b028360862e83b62db665
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63208904"
---
# <a name="application-errors"></a>Anwendungsfehler

Suchen Sie nach Informationen zu den **AADSTS-Fehlercodes**, die vom Azure Active Directory (Azure AD)-Sicherheitstokendienst (Security Token Service, STS) zurückgegeben werden? Lesen Sie [Azure AD-Authentifizierung- und Autorisierungsfehlercodes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes), um AADSTS-Fehlerbeschreibungen, Korrekturen und einige vorgeschlagene Problemumgehungen zu finden.

Autorisierungsfehler können infolge verschiedener Probleme auftreten, von denen die meisten eine 401- oder 403-Fehlermeldung generieren. Die folgenden Beispiele können zu Autorisierungsfehlern führen:

- Falsche [Flüsse für den Erwerb von Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Schlecht konfigurierte [Berechtigungsumfänge](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Fehlende [Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Um häufige Autorisierungsfehler zu beheben, führen Sie die unten aufgeführten Schritte aus, die dem erhaltenen Fehler am nächsten kommen. Es können mehrere gelten.

**Fehler „401 Unauthorized“: Ist Ihr Token gültig?**

Stellen Sie sicher, dass Ihre Anwendung ein gültiges Zugriffstoken für Microsoft Graph als Teil der Anforderung darstellt. Dieser Fehler bedeutet oft, dass das Zugriffstoken im HTTP-Authentifizierungsanforderungs-Header fehlen kann oder dass das Token ungültig oder abgelaufen ist. Wir empfehlen dringend, für den Erwerb von Zugriffstoken die [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) zu verwenden. Darüber hinaus kann dieser Fehler auftreten, wenn Sie versuchen, ein delegiertes Zugriffstoken zu verwenden, das einem persönlichen Microsoft-Konto gewährt wird, um auf eine API zuzugreifen, die nur Geschäfts- oder Schulkonten (Organisationskonten) unterstützt.

**Fehler „403 Forbidden“: Haben Sie den richtigen Berechtigungssatz ausgewählt?**

Überprüfen Sie, ob Sie den richtigen Satz von Berechtigungen basierend auf den Microsoft Graph APIs angefordert haben, die Ihre App aufruft. Empfohlene Berechtigungen mit den geringsten Rechten werden in allen Themen zur Api-Referenzmethode von Microsoft Graph bereitgestellt. Darüber hinaus müssen diese Berechtigungen durch einen Benutzer oder einen Administrator für die Anwendung gewährt werden. Berechtigungen werden normalerweise über eine Zustimmungsseite oder mithilfe des Anwendungsregistrierungblatts im Azure Portal gewährt. Klicken Sie auf dem Blatt **Einstellungen** für die Anwendung auf **Erforderliche Berechtigungen** und dann auf **Berechtigungen gewähren**.

- [Microsoft Graph-Berechtigungen](https://docs.microsoft.com/graph/permissions-reference) 
- [Grundlegendes zu Azure AD-Berechtigungen und -Zustimmung](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Fehler „403 Forbidden“: Hat Ihre Anwendung ein Token erworben, das den ausgewählten Berechtigungen entspricht?**

Stellen Sie sicher, dass die Art der angeforderten oder gewährten Berechtigungen mit der Art des Zugriffstokens übereinstimmt, das von Ihrer App erworben wird. Möglicherweise fordern Sie Anwendungsberechtigungen an und gewähren diese, verwenden aber delegierte interaktive Codefluss-Token anstelle von Clientanmeldeinformationsfluss-Token, oder Sie fordern delegierte Berechtigungen an und gewähren diese, verwenden aber Clientanmeldeinformationsfluss-Token anstelle delegierter Codefluss-Token.

- [Zugriff im Namen von Benutzern und delegierte Berechtigungen erhalten](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD Version 2.0 – OAuth 2.0 Autorisierungscode-Fluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Zugriff ohne Benutzer (Daemon-Dienst) und Anwendungsberechtigungen erhalten](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD Version 2.0 – OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Fehler „403 Forbidden“: Passwort zurücksetzen**

Derzeit gibt es keine Anwendungsberechtigungs-Daemon-Dienst-zu-Dienst-Berechtigungen, die das Zurücksetzen von Benutzerkennwörtern zulassen. Diese APIs werden nur unter Verwendung der interaktiven delegierten Codeflüsse mit einem angemeldeten Administrator unterstützt.

- [Microsoft Graph-Berechtigungen](https://docs.microsoft.com/graph/permissions-reference)

**„403 Forbidden“: Hat der Benutzer Zugriff und ist er lizenziert?**

Bei delegierten Codeflüssen wertet Microsoft Graph aus, ob die Anforderung basierend auf den Berechtigungen, die der App erteilt wurden, und den Berechtigungen des angemeldeten Benutzers zulässig ist. Dieser Fehler deutet im Allgemeinen darauf hin, dass der Benutzer nicht genügend Rechte besitzt, die Anforderung auszuführen, oder dass der Benutzer nicht für die Daten lizenziert ist, auf die zugegriffen wird. Nur Benutzer mit den erforderlichen Berechtigungen oder Lizenzen können die Anfrage erfolgreich stellen.

**„403 Forbidden“: Haben Sie die richtige Ressourcen-API ausgewählt?**

API-Dienste wie Microsoft Graph überprüfen, ob der Aud-Anspruch (Audience) im empfangenen Zugriffstoken mit dem wert übereinstimmt, den er für sich selbst erwartet, und wenn nicht, führt dies zu einem 403 Forbidden-Fehler. Ein häufiger Fehler, der zu diesem Fehler führt, ist der Versuch, ein für Azure AD-Graph-APIs, Outlook-APIs oder Microsoft Office SharePoint Online-/OneDrive-APIs erworbenes Token zu verwenden, um Microsoft Graph aufzurufen (oder umgekehrt). Stellen Sie sicher, dass die Ressource (oder der Geltungsbereich), für die Ihre Anwendung ein Token erwirbt, mit der API übereinstimmt, die von der Anwendung aufgerufen wird.

**„400 Bad Request“ oder „403 Forbidden“: Entspricht der Benutzer die Richtlinien für den bedingten Zugriff (CA) des Unternehmens?**

Basierend auf den Zertifizierungsstellenrichtlinien einer Organisation kann ein Benutzer, der über Ihre App auf Microsoft Graph Ressourcen zugreift, möglicherweise um zusätzliche Informationen gefragt werden, die nicht im ursprünglich von Ihrer App erworbenen Zugriffstoken vorhanden sind. In diesem Fall empfängt Ihre Anwendung den Fehler „400“ mit *interaction_required* beim Erwerb des Zugriffstokens oder den Fehler „403“ mit *insufficient_claims* beim Aufruf von Microsoft Graph. In beiden Fällen enthält die Fehlerantwort zusätzliche Informationen, die dem autorisierenden Endpunkt vorgewiesen werden können, um den Benutzer um zusätzliche Informationen zu bitten (wie Multi-Faktor-Authentifizierung oder Geräteregistrierung).

- [Behandeln von Problemen mit bedingtem Zugriff mit MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Leitfaden für Entwickler für den bedingten Azure Active Directory-Zugriff](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
