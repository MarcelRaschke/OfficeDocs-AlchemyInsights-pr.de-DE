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
ms.localizationpriority: medium
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 827f72d127dbfe5919633273d2f44f8c05989f9e
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63214665"
---
# <a name="how-to-disable-external-groups"></a>So deaktivieren Sie externe Gruppen

Yammer externe Nachrichten gelten Exchange Transportregeln (ETRs), eine Reihe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden. Um zu verhindern, dass Benutzer externe Gruppen erstellen, müssen Sie eine Exchange Transportregel (ETR) konfigurieren und dann Yammer konfigurieren, um die Exchange Transportregel zu verwenden, um externe Nachrichten zu blockieren.
  
Nachdem Sie eine Regel in Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass sie in Yammer angewendet wird:
  
- Melden Sie sich bei Yammer als bestätigter Administrator an, und wechseln **Sie im Yammer Admin Center** zu C **Content and Security \> Einstellungen.**

- Wählen Sie unter **"Externes Messaging**" **in Yammer die Option "Enforce your Exchange Online Exchange Transport Rules (ETRs) " aus.**

- Wählen Sie **Speichern** aus.

Weitere Informationen finden Sie unter ["Externes Messaging in einem Yammer Netzwerk deaktivieren](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)".
  