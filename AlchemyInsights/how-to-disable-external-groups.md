---
title: So deaktivieren Sie externe Gruppen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 80958f74b16878b9ab4525495b143f3a1814b227
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61940229"
---
# <a name="how-to-disable-external-groups"></a>So deaktivieren Sie externe Gruppen

Yammer externe Nachrichten gelten Exchange Transportregeln (ETRs), einer Reihe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden. Um zu verhindern, dass Benutzer externe Gruppen erstellen, müssen Sie eine Exchange Transportregel (ETR) konfigurieren und dann Yammer konfigurieren, um die Exchange Transportregel zu verwenden, um externe Nachrichten zu blockieren.
  
Nachdem Sie eine Regel im Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass sie in Yammer angewendet wird:
  
- Melden Sie sich bei Yammer als bestätigter Administrator an, und wechseln Sie im **Yammer Admin Center** zu C Content and Security **\> Einstellungen.**

- Wählen Sie unter **"Externes Messaging"** die Option **"Exchange Online Exchange Transportregeln (ETRs) in Yammer erzwingen" aus.**

- Wählen Sie **Speichern** aus.

Weitere Informationen finden Sie unter ["Externes Messaging in einem Yammer Netzwerk deaktivieren".](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  