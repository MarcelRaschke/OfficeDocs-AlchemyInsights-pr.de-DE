---
title: Probleme mit Tokenansprüchen und Attributen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 293f78ff13b5595b1813fd0ae228b8cb5a4a6216
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66352479"
---
# <a name="issues-with-token-claims-and-attributes"></a>Probleme mit Tokenansprüchen und Attributen

**Aktualisieren, Konfigurieren oder Entfernen von Tokenansprüchen**

1. Mithilfe von Azure Active Directory (Azure AD) können Sie [den Anspruchstyp für den Rollenanspruch](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) im Antworttoken anpassen, das Sie nach der Autorisierung einer App erhalten.
2. Anwendungsentwickler können optionale Ansprüche in ihren Azure AD-Anwendungen verwenden, um anzugeben, welche Ansprüche sie in Token angeben möchten, die an ihre Anwendung gesendet werden. Weitere Informationen finden Sie unter [Bereitstellen optionaler Ansprüche für Ihre App](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurieren sie Gruppenansprüche für Anwendungen mit Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Wenn Sie nahtloses einmaliges Anmelden in Ihrer Anwendung verwenden, finden Sie [informationen zum Anpassen von Ansprüchen, die im SAML-Token für Unternehmensanwendungen ausgegeben wurden](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Anspruchsattributzuordnung**

1. Informationen zum Konfigurieren der Anspruchszuordnungsrichtlinie mithilfe von PowerShell finden [Sie unter Anpassen von Ansprüchen, die in Token für eine bestimmte App in einem Mandanten ausgegeben wurden (Vorschau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Verzeichnisschemaerweiterungsattribute bieten eine Möglichkeit, zusätzliche Daten in Azure Active Directory auf Benutzerobjekten und anderen Verzeichnisobjekten wie Gruppen, Mandantendetails, Dienstprinzipalen zu speichern. Nur Erweiterungsattribute für Benutzerobjekte können zum Ausgeben von Ansprüchen an Anwendungen verwendet werden. [Die Verwendung von Verzeichnisschemaerweiterungsattributen in Ansprüchen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) beschreibt, wie Verzeichnisschemaerweiterungsattribute zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen verwendet werden.

Weitere Informationen zu Tokenansprüchen finden Sie unter:

- [Ansprüche in Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Ansprüche in einem id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Ansprüche](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , die Sie in ID-Token und Zugriffstoken erwarten können, die von Azure AD B2C ausgestellt wurden
- [SAML-Tokenanspruchsreferenz](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
