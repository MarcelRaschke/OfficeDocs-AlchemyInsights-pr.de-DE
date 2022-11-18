---
title: Konfigurieren des nahtlosen einmaligen Anmeldens (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 33793e453c89114d31bdb9ab93939df6fd4dabae
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66392907"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurieren des nahtlosen einmaligen Anmeldens (SSO)

**Konfigurieren von Anwendungen**

1. Sie sollten die Werte vom Anwendungsanbieter abrufen. Sie können die Werte manuell eingeben oder eine Metadatendatei hochladen, um den Wert der Felder zu extrahieren.
2. Viele Apps wurden bereits für die Arbeit mit Azure AD vorkonfiguriert. Diese Apps werden im Katalog der Apps aufgeführt, die Sie durchsuchen können, wenn Sie Ihrem Azure AD-Mandanten eine App hinzufügen. Die [Schnellstartserie](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) führt Sie durch den Prozess.
3. Um eine Nicht-Kataloganwendung zu erstellen, können Sie auf **die Schaltfläche "Eigene Anwendung erstellen** " klicken und Ihrer Anwendung einen Namen geben.
    - Standardmäßig wird die Option " **Alle anderen Anwendungen integrieren" ausgewählt, die Sie im Katalog nicht finden** . Dies ist die richtige Option für Nicht-Kataloganwendungen.
    - Sobald Sie auf **"Erstellen"** klicken, nachdem Sie den Namen für die Anwendung eingegeben haben, wird eine neue Nicht-Katalog-Enterprise-Anwendung erstellt.
    - Anschließend können Sie unter **"Verwalten** dieser Anwendung" zum **einmaligen Anmelden** navigieren, und Sie können verschiedene Techniken für die Implementierung in Ihrer Umgebung sehen.

**Konfigurieren eines nahtlosen SSO für eine bestimmte Anwendung**

Für die Apps in der Galerie finden Sie detaillierte, schrittweise Anleitungen. Um auf die Schritte zuzugreifen, können Sie eine Liste aller Lernprogramme zur App-Konfiguration in [SaaS-App-Konfigurationslernprogrammen](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) durchsuchen.

**Konfigurieren von SAML-basiertem SSO**

1. [Schnellstart: Einrichten von SAML-basiertem einmaligem Anmelden (Single Sign-On, SSO) für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Weitere Informationen zur SAML-basierten Option für einmaliges Anmelden finden [Sie unter Grundlegendes zum SAML-basierten einmaligen Anmelden](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Informationen zu den SAML 2.0-Authentifizierungsanforderungen und -Antworten, die Azure Active Directory (Azure AD) für single Sign-On (SSO) unterstützt, finden Sie unter [Single Sign-On SAML-Protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Informationen zum Erstellen und Konfigurieren eines SAML-basierten einmaligen Anmeldens (Single Sign-On, SSO) für Ihre Anwendung in Azure Active Directory (Azure AD) mithilfe der Microsoft Graph-API finden Sie unter [Konfigurieren des SAML-basierten einmaligen Anmeldens für Ihre Anwendung mithilfe der Microsoft Graph-API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Informationen zur Verwendung des SAML-Protokolls durch Azure AD finden Sie unter [Verwendung des SAML-Protokolls durch die Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurieren von Token und Ansprüchen**

1. [Vorgehensweise: Anpassen von Ansprüchen, die im SAML-Token für Unternehmensanwendungen ausgegeben wurden](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Informationen zum Konfigurieren von Ansprüchen mithilfe von PowerShell finden Sie unter [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Informationen zum Konfigurieren optionaler Ansprüche finden Sie unter [How to: Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Informationen zum Verwenden von Verzeichnisschemaerweiterungsattributen zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen finden [Sie unter Verwenden von Verzeichnisschemaerweiterungsattributen in Ansprüchen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Informationen zum Konfigurieren der Tokenlebensdauer finden Sie [unter konfigurierbare Tokenlebensdauern in der Microsoft Identity Platform (Vorschau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurieren von Richtlinien für die Tokenlebensdauer (Vorschau)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – In diesem Artikel wird ein allgemeines Richtlinienszenario beschrieben, das Ihnen helfen kann, neue Regeln für die Tokenlebensdauer aufzuerlegen. In dem Beispiel erfahren Sie, wie Sie eine Richtlinie erstellen, die erfordert, dass Benutzer sich häufiger in Ihrer Web-App authentifizieren.

**Problembehandlung bei der SSO-Konfiguration**

- Häufig gestellte Fragen zu Azure Active Directory Seamless Single Sign-On (Seamless SSO) finden Sie unter [Azure Active Directory Seamless Single Sign-On: Häufig gestellte Fragen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informationen zur Problembehandlung bei häufig auftretenden Problemen im Zusammenhang mit Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO) finden Sie unter [Problembehandlung beim nahtlosen einmaligen Anmelden in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
