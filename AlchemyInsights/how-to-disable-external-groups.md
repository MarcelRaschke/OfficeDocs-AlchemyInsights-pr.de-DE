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
ms.openlocfilehash: b4d95d7f7061d7aac2ed65e94f9328fbbe534924
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62684879"
---
# <a name="how-to-disable-external-groups"></a>So deaktivieren Sie externe Gruppen

Yammer externe Nachrichten gelten Exchange Transportregeln (ETRs), einer Reihe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden. Um zu verhindern, dass Benutzer externe Gruppen erstellen, müssen Sie eine Exchange Transportregel (ETR) konfigurieren und dann Yammer so konfigurieren, dass die Exchange-Transportregel verwendet wird, um externe Nachrichten zu blockieren.
  
Nachdem Sie eine Regel im Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass sie in Yammer angewendet wird:
  
- Melden Sie sich bei Yammer als bestätigter Administrator an, und wechseln Sie im **Yammer Admin Center** zu C **Content and Security \> Einstellungen.**

- Wählen Sie unter **"Externes Messaging**" **in Yammer die Option "Erzwingen Ihrer Exchange Online Exchange Transportregeln (ETRs) aus.**

- Wählen Sie **Speichern** aus.

Weitere Informationen finden Sie unter ["Externes Messaging in einem Yammer Netzwerk deaktivieren](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)".
  