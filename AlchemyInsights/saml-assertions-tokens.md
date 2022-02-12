---
title: SAML Assertions (Tokens)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: d443f48e32d449ab367831595e4a9dae99768662
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62597998"
---
# <a name="saml-assertions-tokens"></a>SAML Assertions (Tokens)

1. SAML-Token (Security Assertions Markup Language) sind XML-Darstellungen von Ansprüchen. Standardmäßig werden SAML-Token, die Windows Communication Foundation (WCF) in Verbundsicherheitsszenarien verwendet wird, als Token ausgegeben. Weitere Informationen finden Sie unter [SAML-Token und -Ansprüche](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Die Microsoft Identity Platform gibt bei der Verarbeitung jedes Authentifizierungsflusses mehrere Arten von Sicherheitstoken aus. Die [SAML-Tokenanspruchsreferenz](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beschreibt das Format, die Sicherheitsmerkmale und den Inhalt von SAML 2.0-Token.
3. Befolgen Sie die Anleitungen in [konfigurierbaren Tokenlebensdauern in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes), um zu verstehen, wie Tokenlebensdauern konfiguriert werden.
4. Führen Sie die in [diesem Artikel](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) beschriebenen Schritte aus, um zu verstehen, wie sie Azure AD SAML-Tokenverschlüsselung konfigurieren.
5. In Azure AD können Sie Zertifikatsignierungsoptionen und den Zertifikatsignierungsalgorithmus einrichten. Weitere Informationen finden Sie unter ["Erweiterte Zertifikatsignierungsoptionen" im SAML-Token für Katalog-Apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
