---
title: Problembehandlung der Sicherheitstipp für Überprüfungen der Betrugserkennung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 64dcfd4440f48739fca7e4fbd14dc0c4130f7de5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63229713"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problembehandlung der Sicherheitstipp für Überprüfungen der Betrugserkennung

Wenn Sie eine Sicherheitstipp mit der Meldung "Der Absender hat unsere Betrugserkennungsprüfungen nicht bestanden und möglicherweise nicht die Person, die er zu sein scheint" erhalten, hat der Absender die DKIM- oder SPF-Authentifizierungsprüfungen nicht bestanden. Die beste Methode, um dies zu beheben, besteht darin, dass der Absender sich selbst autorisiert. Wenn der Absender in Ihrem Auftrag sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.
  
Weitere Informationen finden Sie unter [Problembehandlung der roten (verdächtigen) Sicherheitstipp für Überprüfungen der Betrugserkennung](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/).
  
Hier sind einige weitere Links, die Ihnen helfen können:
  
- [Wie Microsoft das Absenderrichtlinienframework (SPF) verwendet, um Spoofing zu verhindern](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Einrichten von SPF zum Verhindern von Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
