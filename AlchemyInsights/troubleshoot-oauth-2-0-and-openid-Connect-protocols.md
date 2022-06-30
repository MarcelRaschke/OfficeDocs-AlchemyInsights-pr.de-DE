---
title: Behandeln von Problemen mit OAuth 2.0- und OpenID Connect-Protokollen
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
- "9776"
ms.date: 03/17/2021
ms.openlocfilehash: 120903dcfba95480e1abce61d90df15c6df8341c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66371307"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Behandeln von Problemen mit OAuth 2.0- und OpenID Connect-Protokollen

Führen Sie die folgenden empfohlenen Schritte aus, um Probleme mit OAuth 2.0 und OpenID Connect zu beheben:

Weitere Informationen finden Sie in den folgenden Artikeln zur Konfiguration und Problembehandlung von OAuth 2.0- und OpenID Connect-Protokollen:

- [Microsoft Identity Platform und OAuth 2.0 Autorisierungscodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow): In diesem Artikel wird die direkte Programmierung in einer beliebigen Sprache für den **Code-Genehmigungsablauf (PKCE)** in Ihrer Anwendung erläutert.
- [Microsoft Identity Platform und der OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow): In diesem Artikel wird beschrieben, wie Sie direkt für den **Clientanmeldeinformationsfluss** in Ihrer Anwendung programmieren können.
- [Microsoft Identity Platform und OAuth 2.0-Anmeldeinformationen des Ressourcenbesitzers (ROPC, Resource Owner Password Credentials)](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc): In diesem Artikel wird beschrieben, wie Sie direkt für den **ROPC-Ablauf** programmieren können.
    - Die Microsoft Identity Platform unterstützt nur ROPC für Azure AD-Mandanten und nicht für persönliche Konten. Dies bedeutet, dass Sie einen mandantenspezifischen Endpunkt `**(https://login.microsoftonline.com/{TenantId_or_Name})**` oder den **Organisations**-Endpunkt verwenden müssen.
    - Persönliche Konten, die zu einem Azure AD-Mandanten eingeladen wurden, können kein ROPC verwenden.
    - Konten, die nicht über Kennwörter verfügen, können sich nicht über ROPC anmelden. Für dieses Szenario empfehlen wir, stattdessen einen anderen Ablauf für Ihre App zu verwenden.
    - Wenn Benutzer sich mittels [mehrstufiger Authentifizierung (Multi-Factor Authentication, MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) bei der Anwendung anmelden müssen, werden sie blockiert.
    - ROPC wird in [Hybrididentitätsverbund](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed)-Szenarien nicht unterstützt (z. B. Azure AD und ADFS, die für die Authentifizierung von lokalen Konten verwendet werden). Wenn Benutzer ganzseitig auf einen lokalen Identitätsanbieter umgeleitet werden, kann Azure AD den Benutzernamen und das Kennwort für diesen Identitätsanbieter nicht testen. [Pass-Through-Authentifizierung](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) mit ROPC wird jedoch unterstützt.
    - Eine Ausnahme von einem Hybrididentitätsverbundszenario wäre Folgendes: Die Home Realm Discovery-Richtlinie mit **AllowCloudPasswordValidation** auf **TRUE** ermöglicht den ROPC-Fluss für Verbundbenutzer, wenn das lokale Kennwort mit der Cloud synchronisiert wird. Weitere Informationen finden Sie unter [Aktivieren der direkten ROPC-Authentifizierung von Verbundbenutzern für Legacyanwendungen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications). 
- [Microsoft Identity Platform und OAuth 2.0 "Im Auftrag von"-Ablauf](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow): In diesem Artikel die direkte Programmierung für den **"Im Auftrag von"-Ablauf (On-Behalf-Of, OBO)** in Ihrer Anwendung erläutert.
- [Microsoft Identity Platform und OpenID Connect-Protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc): In diesem Artikel wird gezeigt, wie das OpenID-Protokoll sprachunabhängig implementiert wird, und beschrieben, wie HTTP-Nachrichten gesendet und empfangen werden können, ohne irgendwelche Open-Source-Bibliotheken von Microsoft zu verwenden.

**Zugriffstoken**

[Zugriffstoken von Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens): Erfahren Sie, wie Ihre API die Ansprüche in einem Zugriffstoken validieren und verwenden kann. Die gesamte Dokumentation in diesem Artikel gilt, sofern nicht anders angegeben, nur für Token, die für von Ihnen registrierte APIs ausgestellt wurden. Sie gilt nicht für Token, die für Microsoft-eigene APIs ausgestellt wurden, noch können diese Token verwendet werden, um zu überprüfen, wie Microsoft Identity Platform-Token für eine von Ihnen erstellte API ausstellt.

**Anwendungskonfiguration**

[Einschränkungen für Umleitungs-URI (Antwort-URLs)](https://docs.microsoft.com/azure/active-directory/develop/reply-url): Erfahren Sie, wie Sie den Umleitungs-URI (Antwort-URL) konfigurieren können. Ein Umleitungs-URI (oder Antwort-URL) ist der Ort, an den der Autorisierungsserver den Benutzer weiterleitet, sobald die App erfolgreich autorisiert wurde und einen Autorisierungscode oder ein Zugriffstoken erhalten hat. Der Autorisierungsserver sendet den Code oder das Token an den Umleitungs-URI. Daher ist es wichtig, dass Sie im Rahmen der App-Registrierung die richtige Adresse registrieren.

**Bereitstellung der Anwendung**

[Lernprogramm: Entwickeln und Planen der Bereitstellung für einen SCIM-Endpunkt](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups): In diesem Artikel wird beschrieben, wie Sie einen SCIM-Endpunkt erstellen und in den AAD-Bereitstellungsdienst integrieren können.


