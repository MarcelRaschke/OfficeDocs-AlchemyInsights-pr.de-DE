---
title: SAML Assertions (Tokens)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 2af183f71e15540e9b93a0fda824c56838787120
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66291439"
---
# <a name="saml-assertions-tokens"></a>SAML Assertions (Tokens)

1. SAML-Token (Security Assertions Markup Language) sind XML-Darstellungen von Ansprüchen. Standardmäßig werden SAML-Token, die Windows Communication Foundation (WCF) in Verbundsicherheitsszenarien verwendet, token ausgegeben. Weitere Informationen finden Sie unter [SAML-Token und -Ansprüche](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Die Microsoft Identity Platform gibt bei der Verarbeitung jedes Authentifizierungsflusses mehrere Arten von Sicherheitstoken aus. [Die SAML-Tokenanspruchsreferenz](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beschreibt das Format, die Sicherheitsmerkmale und den Inhalt von SAML 2.0-Token.
3. Befolgen Sie die [Anleitungen in konfigurierbaren Tokenlebensdauern in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes), um zu verstehen, wie Tokenlebensdauern konfiguriert werden.
4. Führen Sie die in [diesem Artikel](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) beschriebenen Schritte aus, um zu verstehen, wie Sie die Azure AD SAML-Tokenverschlüsselung konfigurieren.
5. In Azure AD können Sie Optionen für die Zertifikatsignierung und den Zertifikatsignierungsalgorithmus einrichten. Weitere Informationen finden Sie [unter Erweiterte Zertifikatsignaturoptionen im SAML-Token für Katalog-Apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
