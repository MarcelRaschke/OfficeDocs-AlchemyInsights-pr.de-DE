---
title: Erweiterte Authentifizierungskonzepte für Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003931"
- "9004625"
- "6986"
- "8329"
ms.date: 12/03/2020
ms.openlocfilehash: 40d063928dadfcd162e68c8a7b12fcc4e79d934c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66275917"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Erweiterte Authentifizierungskonzepte für Microsoft Edge

Es folgen die erweiterten Authentifizierungskonzepte, die für Microsoft Edge gelten:

**Proaktive Authentifizierung**

Wenn Sie die [ProactiveAuthEnabled-Richtlinie](https://go.microsoft.com/fwlink/?linkid=2134621) aktivieren, versucht Microsoft Edge, angemeldete Benutzer proaktiv über Microsoft-Dienste zu authentifizieren. In regelmäßigen Abständen wird ein Onlinedienst verwendet, um nach einem aktualisierten Manifest zu suchen, das die Konfiguration für die proaktive Authentifizierung enthält.

Vorteile: Die proaktive Authentifizierung ermöglicht die Authentifizierung bei wichtigen Diensten, z. B. der Office-Seite "Neue Registerkarte". Wenn Bing als Suchmaschine verwendet wird, verbessert die proaktive Authentifizierung außerdem die Leistung der Adressleiste und hilft, Suchergebnisse zu generieren, die an die Anforderungen Ihres Unternehmens angepasst sind.

**Windows Hello CredUI für NTLM-Authentifizierung**

Wenn einmaliges Anmelden (Single Sign-On, SSO) nicht verfügbar ist, wenn eine Website versucht, den Benutzer über den NTLM- oder Negotiate-Mechanismus anzumelden, ermöglicht dieses Feature dem Benutzer, die Betriebssystemanmeldeinformationen für die Website freizugeben und die Authentifizierungs-Herausforderung mithilfe Windows Hello Cred UI zu erfüllen. Dieser Anmeldefluss wird nur in Windows 10 und nur für Benutzer angezeigt, die während einer NTLM- oder Aushandlungs-Abfrage keinen SSO erhalten.

**Automatische Anmeldung mit gespeicherten Kennwörtern**

Benutzer, die Kennwörter in Microsoft Edge speichern, können die automatische Anmeldung bei Websites aktivieren, auf denen sie Anmeldeinformationen gespeichert haben. Benutzer können dieses Feature in edge://settings/passwords aktivieren oder deaktivieren, und Sie können es in den [Kennwort-Manager-Richtlinien](https://go.microsoft.com/fwlink/?linkid=2134622) konfigurieren.
