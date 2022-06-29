---
title: Behandeln von Problemen mit OIDC-basiertem nahtlosen einmaligen Anmelden (Seamless Single Sign-On, SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: c05bfdafb5fb647d232cab5ebe754b177dca4460
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66279802"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Behandeln von Problemen mit OIDC-basiertem nahtlosen einmaligen Anmelden (Seamless Single Sign-On, SSO)

- Informationen zum Hinzufügen einer OIDC-basierten App zu Ihrem [Azure-Mandanten finden Sie in der Schnellstartanleitung: Einrichten von OIDC-basiertem einmaligem Anmelden (Single Sign-On, SSO) für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Weitere Informationen zu Apps, die den OpenID Connect-Standard zum Implementieren des einmaligen Anmeldens verwenden, finden [Sie unter Grundlegendes zum OIDC-basierten einmaligen Anmelden](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Informationen für den Fall, dass Sie Ihren Code schreiben, indem Sie HTTP-Anforderungen direkt senden und verarbeiten oder eine Open-Source-Bibliothek eines Drittanbieters verwenden, anstatt eine unserer Open-Source-Bibliotheken zu verwenden, finden Sie unter [OAuth 2.0 und OpenID Connect-Protokolle auf der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokolle**

1. [Microsoft Identity Platform und impliziter Genehmigungsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – Das definierende Merkmal der impliziten Erteilung ist, dass Token (ID-Token oder Zugriffstoken) direkt vom /authorize-Endpunkt anstelle des /token-Endpunkts zurückgegeben werden. Dies wird häufig als Teil des Autorisierungscodeflusses verwendet, in dem **sogenannten "Hybridfluss" – Abrufen des ID-Tokens für die /authorize-Anforderung zusammen mit einem Autorisierungscode**. In diesem Artikel wird beschrieben, wie Sie direkt mit dem Protokoll in Ihrer Anwendung programmieren, um Token von Azure AD anzufordern.
2. [Microsoft Identity Platform- und OAuth 2.0-Autorisierungscodefluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Die OAuth 2.0-Autorisierungscodegenehmigung kann in Apps verwendet werden, die auf einem Gerät installiert sind, um Zugriff auf geschützte Ressourcen wie Web-APIs zu erhalten. Mithilfe der Microsoft Identity Platform Implementierung von OAuth 2.0 können Sie **Ihren mobilen und Desktop-Apps Anmelde- und API-Zugriff hinzufügen**. In diesem Artikel wird beschrieben, wie Sie mit einer beliebigen Sprache direkt mit dem Protokoll in Ihrer Anwendung programmieren.
3. [Microsoft Identity Platform- und OpenID Connect-Protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Wenn Sie die Implementierung von OpenID Connect durch die Microsoft Identity Platform verwenden, können Sie Ihren Apps Anmelde- und API-Zugriff hinzufügen. In diesem Artikel wird erläutert, wie Sie dies unabhängig von der Sprache tun können, und es wird beschrieben, wie **HTTP-Nachrichten ohne Microsoft Open Source-Bibliotheken gesendet und empfangen** werden.
4. [Microsoft Identity Platform und der Fluss der OAuth 2.0-Clientanmeldeinformationen](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Sie können die in RFC 6749 angegebene OAuth 2.0-Clientanmeldeinformationenerteilung verwenden, die manchmal als **zweibeiniges OAuth** bezeichnet wird, um mithilfe der Identität einer Anwendung auf im Web gehostete Ressourcen zuzugreifen. Diese Art der Gewährung wird häufig für Server-zu-Server-Interaktionen verwendet, die ohne sofortige Interaktion mit einem Benutzer im Hintergrund ausgeführt werden müssen. Diese Arten von Anwendungen werden häufig als **Daemons** oder **Dienstkonten** bezeichnet. In diesem Artikel wird beschrieben, wie Sie direkt mit dem Protokoll in Ihrer Anwendung programmieren.
