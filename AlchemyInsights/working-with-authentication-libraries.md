---
title: Arbeiten mit Authentifizierungsbibliotheken
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f2f401622253e6b2c3da14bf88deeecdc1353d6b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63279953"
---
# <a name="working-with-authentication-libraries"></a>Arbeiten mit Authentifizierungsbibliotheken

Um das Problem mit der Microsoft-Authentifizierungsbibliotheken (MSAL) zu beheben, führen Sie die folgenden empfohlenen Schritte durch:

1. **Arbeiten mit MSAL**: [Microsoft Identity Platform-Authentifizierungsbibliotheken](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – In diesem Artikel wird die Unterstützung der Microsoft-Authentifizierungsbibliothek für verschiedene Anwendungstypen beschrieben. Er enthält Links zum Quellcode der Bibliothek, gibt an, wo Sie das Paket für das Projekt Ihrer App erhalten und ob die Bibliothek die Benutzeranmeldung (Authentifizierung), den Zugriff auf geschützte Web-APIs (Autorisierung) oder beides unterstützt.

2. **Problembehandlung**: MSAL unterstützt mehrere Authentifizierungsabläufe zur Verwendung in verschiedenen Anwendungsszenarien. Je nachdem, wie Ihre Clientanwendung aufgebaut ist, kann die MSAL einen oder mehrere der von Microsoft Identity Platform unterstützten Authentifizierungsabläufe verwenden. Diese Abläufe können verschiedene Arten von Token und Autorisierungscodes erzeugen und erfordern unterschiedliche Token, damit sie funktionieren.

3. **Zugriffstoken**: [Zugriffstoken von Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Erfahren Sie, wie Ihre API die Ansprüche in einem Zugriffstoken validieren und verwenden kann. Die gesamte Dokumentation in diesem Artikel gilt, sofern nicht anders angegeben, nur für Token, die für von Ihnen registrierte APIs ausgestellt wurden. Sie gilt nicht für Token, die für Microsoft-eigene APIs ausgestellt wurden, noch können diese Token verwendet werden, um zu überprüfen, wie Microsoft Identity Platform Token für eine von Ihnen erstellte API ausstellt.

**Ende der Unterstützung für die Azure Active Directory-Authentifizierungsbibliothek (ADAL)**

- **Seit dem 30. Juni 2020** werden keine neuen Features mehr zu ADAL und Azure AD Graph hinzugefügt. Wir werden weiterhin technischen Support und Sicherheitsupdates bereitstellen, jedoch keine Funktionsupdates mehr.
- **Ab dem 30. Juni 2022** werden wir den Support für ADAL und Azure AD Graph beenden und keinen technischen Support oder Sicherheitsupdates mehr bereitstellen.
- Apps, die ADAL unter vorhandenen Betriebssystemversionen verwenden, funktionieren auch nach diesem Zeitpunkt weiterhin, *es werden jedoch weder Support noch Sicherheitsupdates dafür bereitgestellt*.
- Apps, die Azure AD Graph nach dieser Zeit verwenden, empfangen möglicherweise keine Antworten mehr vom Azure AD Graph-Endpunkt.

**ADAL-Migration**

- Es wird ein Update auf die MSAL empfohlen, die über die neuesten Features und Sicherheitsupdates verfügt.
- Wenn Sie Microsoft-Apps verwenden, sollten Sie wissen, dass Microsoft dabei ist, Microsoft-Apps bis zum Stichtag des Endes des Supports zu MSAL zu migrieren, um sicherzustellen, dass sie von den laufenden Sicherheits- und Featureverbesserungen von MSAL profitieren.

1. [Lesen Sie hierzu die häufig gestellten Fragen zu ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Informationen zum Migrieren von Apps nach Plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Wenn Sie nach dem Lesen des Leitfadens für die Plattform Ihrer App weitere Fragen haben, können Sie diese unter [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) mit dem Tag „[azure-ad-adal-deprecation]“ posten oder ein Problem im GitHub-Repository der Bibliothek melden. Im Abschnitt [Sprachen und Frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) des Artikels **Übersicht über die MSAL** finden Sie Links zu den einzelnen Repositorys der Bibliothek.
4. **Wenn Sie Hilfe benötigen, um zu verstehen, welche Ihrer Apps ADAL verwenden**, empfehlen wir Ihnen, den Quellcode all Ihrer Apps zu überprüfen. Wenden Sie sich ggf. an unabhängige Softwareanbieter (ISVs) oder App-Anbieter. Der Microsoft-Support kann Ihnen auch eine Liste aller Nicht-Microsoft ADAL-Apps in Ihrem Mandanten bereitstellen.







