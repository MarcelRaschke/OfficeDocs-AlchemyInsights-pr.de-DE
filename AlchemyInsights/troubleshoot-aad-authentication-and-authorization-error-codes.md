---
title: Behandeln von Problemen mit Azure AD Authentifizierungs- und Autorisierungsfehlercodes (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898310"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Behandeln von Problemen mit Azure AD Authentifizierungs- und Autorisierungsfehlercodes (AADSTS)

Führen Sie die folgenden empfohlenen Schritte aus, um AAD-Authentifizierungs- und Autorisierungsfehlercodes (AADSTS) zu beheben:

1. **Umgang mit Fehlercodes in Ihrer Anwendung**

- Die **OAuth2.0-Spezifikation** https://tools.ietf.org/html/rfc6749#section-5.2enthält Anleitungen dazu, wie Fehler während der Authentifizierung anhand des Fehlerbereichs der Fehlerantwort behandelt werden.

    - **Fehler**: Eine Fehlercodezeichenfolge, mit der auftretende Fehlern klassifiziert werden können, und mit der auf Fehler reagiert werden soll.
    - Das **Fehlerfeld** enthält mehrere mögliche Werte. Weitere Informationen zu bestimmten Fehlern und deren Reaktion finden Sie unter den Protokolldokumentationslinks und OAuth 2.0-Spezifikationen.

- Hier ist eine Beispielfehlerantwort:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Aktuelle Fehlercodeinformationen nachschlagen**

- Fehlercodes und -Meldungen können sich ändern. Die neuesten Informationen finden Sie auf der https://login.microsoftonline.com/error Seite mit AADSTS-Fehlerbeschreibungen, Korrekturen und einigen Vorschlägen, wie Sie die Probleme umgehen können.
- Sie können auch nach [AADSTS-Fehlercodes ](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes), die im Artikel [Azure AD-Authentifizierungs- und Autorisierungsfehlercodes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application) aufgelistet sind, suchen und diese beheben.

3. **Hilfe anfordern**

- [Support- und Hilfeoptionen für Entwickler](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – Wenn Sie eine Antwort auf eine Frage oder Hilfe bei der Lösung eines Problems benötigen, das in unserer Dokumentation nicht behandelt wird, ist es möglicherweise an der Zeit, sich an Experten wenden. Dieser Artikel enthält mehrere Vorschläge, wie Sie beim Entwickeln von Apps, die in die Microsoft Identity Platform für Entwickler integriert sind, Antworten auf Ihre Fragen erhalten.








