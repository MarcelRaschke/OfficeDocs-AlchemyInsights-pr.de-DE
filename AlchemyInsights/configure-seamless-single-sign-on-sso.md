---
title: Konfigurieren des nahtlosen einmaligen Anmeldens (Single Sign-On, SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966036"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurieren des nahtlosen einmaligen Anmeldens (Single Sign-On, SSO)

**Konfigurieren von Anwendungen**

1. Sie sollten die Werte vom Anwendungsanbieter abrufen. Sie können die Werte manuell eingeben oder eine Metadatendatei hochladen, um den Wert der Felder zu extrahieren.
2. Viele Apps wurden bereits für die Verwendung mit Azure AD vorkonfiguriert. Diese Apps sind im Katalog der Apps aufgeführt, die Sie durchsuchen können, wenn Sie Ihrem Azure AD-Mandanten eine App hinzufügen. Die [Schnellstartreihe](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) führt Sie durch den Prozess.
3. Um eine Nicht-Kataloganwendung zu erstellen, können Sie auf die Schaltfläche **"Eigene Anwendung erstellen"** klicken und ihrer Anwendung einen Namen geben.
    - Standardmäßig wird die Option "Alle anderen Anwendungen integrieren" auswählen, **die Sie im Katalog nicht finden. Dies** ist die richtige Option für Nicht-Kataloganwendungen.
    - Sobald Sie nach dem Einfügen des Namens für die Anwendung auf **"Erstellen"** klicken, wird ein neuer Nicht-Katalog Enterprise Anwendung erstellt.
    - Dann können Sie unter **"Verwalten** dieser Anwendung" zu **Single Sign-On** navigieren, und Sie können verschiedene Techniken für die Implementierung in Ihrer Umgebung sehen.

**Konfigurieren des nahtlosen SSO für eine bestimmte Anwendung**

Für die Apps in der Galerie finden Sie detaillierte Schritt-für-Schritt-Anweisungen. Um auf die Schritte zuzugreifen, können Sie eine Liste aller Lernprogramme zur App-Konfiguration in [SaaS-App-Konfigurationslernprogrammen](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)durchsuchen.

**Konfigurieren von SAML-basiertem SSO**

1. [Schnellstart: Richten Sie SAML-basiertes einmaliges Anmelden (Single Sign-On, SSO) für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)ein.
2. Weitere Informationen zur SAML-basierten Option für einmaliges Anmelden finden Sie unter [Grundlegendes zum SAML-basierten einmaligen Anmelden.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Informationen zu den SAML 2.0-Authentifizierungsanforderungen und -antworten, die Azure Active Directory (Azure AD) für Single Sign-On (SSO) unterstützt, finden Sie unter [Single Sign-On SAML protocol.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Informationen zum Erstellen und Konfigurieren eines SAML-basierten einmaligen Anmeldens (Single Sign-On, SSO) für Ihre Anwendung in Azure Active Directory (Azure AD) mithilfe der Microsoft Graph-API finden Sie unter Konfigurieren des [SAML-basierten einmaligen Anmeldens für Ihre Anwendung mithilfe der Microsoft Graph-API.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Informationen dazu, wie Azure AD das SAML-Protokoll verwendet, finden Sie unter ["Verwenden des SAML-Protokolls durch das Microsoft Identity Platform".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurieren von Token und Ansprüchen**

1. [How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Informationen zum Konfigurieren von Ansprüchen mithilfe von PowerShell finden Sie unter [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Informationen zum Konfigurieren optionaler Ansprüche finden Sie unter [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Informationen zum Verwenden von Verzeichnisschemaerweiterungsattributen zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen finden Sie unter [Verwenden von Verzeichnisschemaerweiterungsattributen in Ansprüchen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Informationen zum Konfigurieren der Tokenlebensdauer finden Sie unter ["Konfigurierbare Tokenlebensdauern" im Microsoft Identity Platform (Vorschau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurieren von Tokenlebensdauerrichtlinien (Vorschau)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – In diesem Artikel werden wir durch ein allgemeines Richtlinienszenario geführt, das Ihnen dabei helfen kann, neue Regeln für die Tokenlebensdauer festzulegen. In diesem Beispiel erfahren Sie, wie Sie eine Richtlinie erstellen, die erfordert, dass Benutzer sich häufiger in Ihrer Web-App authentifizieren.

**Problembehandlung bei der SSO-Konfiguration**

- Häufig gestellte Fragen zu Azure Active Directory nahtlosen single Sign-On (Seamless SSO) finden Sie unter [Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informationen zur Problembehandlung bei allgemeinen Problemen im Zusammenhang mit Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO) finden Sie unter [Troubleshoot Azure Active Directory Seamless Single Sign-On.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
