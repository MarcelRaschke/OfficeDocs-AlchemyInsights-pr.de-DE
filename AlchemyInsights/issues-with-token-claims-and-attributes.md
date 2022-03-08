---
title: Probleme mit Tokenansprüchen und Attributen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: b5399abb66cfd1a3e575ce758ca871f47c8ac5e6
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63202424"
---
# <a name="issues-with-token-claims-and-attributes"></a>Probleme mit Tokenansprüchen und Attributen

**Aktualisieren, Konfigurieren oder Entfernen von Tokenansprüchen**

1. Mit Azure Active Directory (Azure AD) können Sie [den Anspruchstyp für den Rollenanspruch](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) im Antworttoken anpassen, das Sie erhalten, nachdem Sie eine App autorisiert haben.
2. Anwendungsentwickler können optionale Ansprüche in ihren Azure AD Anwendungen verwenden, um anzugeben, welche Ansprüche in Token an ihre Anwendung gesendet werden sollen. Weitere Informationen finden Sie unter [Bereitstellen optionaler Ansprüche für Ihre App](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurieren von Gruppenansprüchen für Anwendungen mit Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Wenn Sie nahtloses einmaliges Anmelden in Ihrer Anwendung verwenden, lesen Sie [die Informationen zum Anpassen von Ansprüchen, die im SAML-Token für Unternehmensanwendungen ausgegeben wurden](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Anspruchsattributzuordnung**

1. Informationen zum Konfigurieren der Anspruchszuordnungsrichtlinie mithilfe von PowerShell finden Sie unter [Anpassen von Ansprüchen, die in Token für eine bestimmte App in einem Mandanten ausgegeben werden (Vorschau).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Verzeichnisschemaerweiterungsattribute bieten eine Möglichkeit, zusätzliche Daten in Azure Active Directory für Benutzerobjekte und andere Verzeichnisobjekte wie Gruppen, Mandantendetails, Dienstprinzipale zu speichern. Nur Erweiterungsattribute für Benutzerobjekte können verwendet werden, um Ansprüche an Anwendungen zu überweisen. [Die Verwendung von Verzeichnisschemaerweiterungsattributen in Ansprüchen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) beschreibt, wie Verzeichnisschemaerweiterungsattribute zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen verwendet werden.

Weitere Informationen zu Tokenansprüchen finden Sie unter:

- [Ansprüche in Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Ansprüche in einer id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Ansprüche](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims), die Sie in ID-Token und Zugriffstoken erwarten können, die von Azure AD B2C ausgestellt wurden
- [SAML-Tokenanspruchsreferenz](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
