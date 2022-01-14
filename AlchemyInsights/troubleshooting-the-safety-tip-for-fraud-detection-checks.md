---
title: Problembehandlung der Sicherheitstipp für Betrugserkennungsprüfungen
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 658e18b36bb01ac57cffc6daedf7f7c52ca76aba
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61986997"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problembehandlung der Sicherheitstipp für Betrugserkennungsprüfungen

Wenn Sie eine Sicherheitstipp erhalten, die besagt, dass "Der Absender hat unsere Betrugserkennungsprüfungen nicht bestanden hat und möglicherweise nicht die Person ist, die er zu sein scheint", hat der Absender die DKIM- oder SPF-Authentifizierungsprüfungen nicht bestanden. Die beste Methode, um dies zu beheben, besteht darin, dass der Absender sich selbst autorisiert. Wenn der Absender in Ihrem Auftrag sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.
  
Weitere Informationen finden Sie unter [Problembehandlung der roten (verdächtigen) Sicherheitstipp für Überprüfungen der Betrugserkennung.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
Hier sind einige weitere Links, die Ihnen helfen können:
  
- [Wie Microsoft das Absenderrichtlinienframework (SPF) verwendet, um Spoofing zu verhindern](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Einrichten von SPF zum Verhindern von Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
