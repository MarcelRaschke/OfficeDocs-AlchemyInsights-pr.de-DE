---
title: Problembehandlung der Sicherheitstipp für Betrugserkennungsprüfungen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955965"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problembehandlung der Sicherheitstipp für Betrugserkennungsprüfungen

Wenn Sie eine Sicherheitstipp mit der Meldung "Der Absender hat unsere Betrugserkennungsprüfungen nicht bestanden und möglicherweise nicht die Person, die er zu sein scheint" erhalten, hat der Absender die DKIM- oder SPF-Authentifizierungsprüfungen nicht bestanden. Die beste Methode, um dies zu beheben, besteht darin, dass der Absender sich selbst autorisiert. Wenn der Absender in Ihrem Auftrag sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.
  
Weitere Informationen finden Sie unter [Problembehandlung der roten (verdächtigen) Sicherheitstipp für Überprüfungen der Betrugserkennung.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
Hier sind einige weitere Links, die Ihnen helfen können:
  
- [Wie Microsoft das Absenderrichtlinienframework (SPF) verwendet, um Spoofing zu verhindern](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Einrichten von SPF zum Verhindern von Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
