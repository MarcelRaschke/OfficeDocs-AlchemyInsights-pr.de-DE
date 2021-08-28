---
title: Erweiterte Authentifizierungskonzepte für Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934364"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Erweiterte Authentifizierungskonzepte für Microsoft Edge

Es folgen die erweiterten Authentifizierungskonzepte, die für Microsoft Edge gelten:

**Proaktive Authentifizierung**

Wenn Sie die [ProactiveAuthEnabled-Richtlinie](https://go.microsoft.com/fwlink/?linkid=2134621) aktivieren, versuchen Microsoft Edge, angemeldete Benutzer proaktiv über Microsoft-Dienste zu authentifizieren. In regelmäßigen Abständen wird ein Onlinedienst verwendet, um nach einem aktualisierten Manifest zu suchen, das die Konfiguration für die proaktive Authentifizierung enthält.

Vorteile: Die proaktive Authentifizierung ermöglicht die Authentifizierung bei wichtigen Diensten, z. B. der Office Seite "Neue Registerkarte". Wenn Bing als Suchmaschine verwendet wird, verbessert die proaktive Authentifizierung außerdem die Leistung der Adressleiste und hilft bei der Generierung von Suchergebnissen, die an die Anforderungen Ihres Unternehmens angepasst sind.

**Windows Hello CredUI für ntlm-Authentifizierung**

Wenn einmaliges Anmelden (Single Sign-On, SSO) nicht verfügbar ist, wenn eine Website versucht, den Benutzer über ntlm oder den Aushandlungsmechanismus anzumelden, ermöglicht dieses Feature dem Benutzer, die BS-Anmeldeinformationen für die Website freizugeben und die Authentifizierungsanforderung mithilfe Windows Hello Cred UI zu erfüllen. Dieser Anmeldefluss wird nur in Windows 10 und nur für Benutzer angezeigt, die während einer NTLM- oder Einer Negotiate-Abfrage kein SSO erhalten.

**Verwenden von gespeicherten Kennwörtern zum automatischen Anmelden**

Benutzer, die Kennwörter in Microsoft Edge speichern, können die automatische Anmeldung bei Websites aktivieren, auf denen sie Anmeldeinformationen gespeichert haben. Benutzer können dieses Feature in edge://settings/passwords aktivieren oder deaktivieren, und Sie können es in den [Kennwort-Manager-Richtlinien](https://go.microsoft.com/fwlink/?linkid=2134622) konfigurieren.
