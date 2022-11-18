---
title: Problembehandlung des Sicherheitstipps für Betrugserkennungsprüfungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100004"
- "275"
ms.date: 04/21/2020
ms.openlocfilehash: 252517a1489f2d7ac64401d1e387e2f51edf68e4
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66304650"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problembehandlung des Sicherheitstipps für Betrugserkennungsprüfungen

Wenn Sie einen Sicherheitstipp erhalten, der besagt: "Der Absender hat unsere Betrugserkennungsprüfungen nicht bestanden und ist möglicherweise nicht die Person, die er zu sein scheint", hat der Absender entweder DKIM- oder SPF-Authentifizierungsprüfungen nicht bestanden. Die beste Methode, um dies zu beheben, ist, dass der Absender sich selbst autorisiert. Wenn der Absender in Ihrem Auftrag sendet, müssen Sie diese autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.
  
Weitere Informationen finden Sie [unter Problembehandlung des roten (verdächtigen) Sicherheitstipps für Betrugserkennungsprüfungen](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Hier sind einige weitere Links, die Ihnen helfen können:
  
- [Wie Microsoft das Sender Policy Framework (SPF) verwendet, um Spoofing zu verhindern](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Einrichten von SPF zum Verhindern von Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
