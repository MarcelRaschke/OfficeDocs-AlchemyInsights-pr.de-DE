---
title: Verwenden von DLP in Transportregeln
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 983d9a4d76b2baac624aeac6d4d8ffbc20605a12
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65732070"
---
# <a name="using-dlp-in-transport-rules"></a>Verwenden von DLP in Transportregeln

Um Microsoft Purview Data Loss Prevention in einen vorhandenen Transport zu integrieren, verwenden Sie die Bedingung "**Wenn die Nachricht...Vertrauliche Informationen...enthält**" in der Transportregeleinstellung.

**Weitere Informationen finden Sie hier:**

- Integrierte DLP-Typen vertraulicher Informationen in Transportregeln: [Integrieren von Regeln für vertrauliche Informationen](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Sie können die Regel mit oder ohne Richtlinientest auch testen, indem Sie die Regel im Testmodus verwenden.  Sie sollten nach der Erstellung der Regel 30 Minuten warten, bevor Sie sie testen.

- Siehe [Nachrichtenflussregel (Transportregel) testen](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).

**Hinweis**: Wenn Sie eine neue DLP-Richtlinie mit Transportregeln im EAC implementieren möchten, verwenden Sie stattdessen [DLP-Richtlinien im Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies).
