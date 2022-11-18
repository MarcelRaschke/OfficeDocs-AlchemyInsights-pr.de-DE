---
title: Standardauthentifizierung
author: IpeTangonan
ms.author: v-ftangonan
manager: anita.danford
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9009992"
- "16751"
ms.date: 02/22/2022
ms.openlocfilehash: 07ebaed822edb3a33920a1fd16c152c554c02de2
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63230790"
---
# <a name="basic-authentication"></a>Standardauthentifizierung

Im september 2021 wurde eine Ankündigung gemacht, dass die Deaktivierung der Standardauthentifizierung für Outlook-, EWS-, RPS-, POP-, IMAP- und EAS-Protokolle in Exchange Online diesen 1. Oktober 2022 sein wird. SMTP-Authentifizierung wird ebenfalls deaktiviert, wenn sie nicht verwendet wird. Neue Microsoft 365 Mandanten werden erstellt, wobei die Standardauthentifizierung bereits deaktiviert ist, da die Sicherheitsstandards aktiviert sind. Vollständige Ankündigung: [Standardauthentifizierung und Exchange Online – Update vom September 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-authentication-and-exchange-online-september-2021-update/ba-p/2772210)

Diese Entscheidung erfordert, dass Kunden von Apps, die die Standardauthentifizierung verwenden, zu Apps wechseln, die die moderne Authentifizierung verwenden. Die moderne Authentifizierung (tokenbasierte OAuth 2.0-Autorisierung) bietet viele Vorteile und Verbesserungen, die dazu beitragen, die Probleme bei der Standardauthentifizierung zu beheben. OAuth-Zugriffstoken haben beispielsweise eine begrenzte verwendbare Lebensdauer und sind spezifisch für die Anwendungen und Ressourcen, für die sie ausgestellt wurden, sodass sie nicht wiederverwendet werden können. Das Aktivieren und Erzwingen der mehrstufigen Authentifizierung (MultiFactor Authentication, MFA) ist auch mit der modernen Authentifizierung einfach.

*Weitere Informationen zum Ende der Standardauthentifizierung in Exchange Online:* [Veraltete Standardauthentifizierung in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/deprecation-of-basic-authentication-exchange-online)

Wir sind für Sie da, wenn Sie weitere Unterstützung benötigen. Wenn Sie **sich mit einem Microsoft-Spezialisten für weitere Hilfe in Verbindung setzen** möchten, wählen Sie "Chat mit einem Microsoft-Spezialisten" aus, und **klicken Sie dann unten auf "Live-Chat** ".
