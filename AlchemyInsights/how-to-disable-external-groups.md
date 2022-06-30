---
title: So deaktivieren Sie externe Gruppen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "6000006"
- "966"
ms.date: 04/21/2020
ms.openlocfilehash: a8469dc009d3c421c265bb15f63c5564086dac73
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66389001"
---
# <a name="how-to-disable-external-groups"></a>So deaktivieren Sie externe Gruppen

Yammer externes Messaging wendet Exchange-Transportregeln (EXCHANGE Transport Rules, ETRs) an, eine Reihe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden. Um Benutzer daran zu hindern, externe Gruppen zu erstellen, müssen Sie eine Exchange-Transportregel (ETR) konfigurieren und dann Yammer so konfigurieren, dass die Exchange-Transportregel zum Blockieren externer Nachrichten verwendet wird.
  
Nachdem Sie eine Regel im Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass es in Yammer angewendet wird:
  
- Melden Sie sich bei Yammer als bestätigter Administrator an, und wechseln Sie im **Yammer Admin Center** zu den **C-Inhalts- und Sicherheitssicherheitseinstellungen \> .**

- Wählen Sie unter **"Externes Messaging****" in Yammer die Option "Erzwingen Ihrer Exchange Online Exchange-Transportregeln (Exchange Transport Rules, ETRs)" aus.**

- Wählen Sie **Speichern** aus.

Weitere Informationen finden Sie unter [Deaktivieren von externem Messaging in einem Yammer-Netzwerk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  