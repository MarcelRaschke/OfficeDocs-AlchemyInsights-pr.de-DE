---
title: Stromversorgungs- oder Akkusymbol fehlt in Windows 10
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: fdb711a0cc07ff42b4e0587382079a32784d2ba6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66374583"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Stromversorgungs- oder Akkusymbol fehlt in Windows 10

Wenn Ihr Windows 10-Gerät über einen Akku verfügt (z.B. einen Laptop oder ein Tablet oder einen über USB an eine USV angeschlossenen PC), wird in der Taskleiste normalerweise neben der Uhr ein Stromversorgungs-/Akkusymbol angezeigt. Beispiel:

![Akkusymbol](media/battery-icon.png)

Wenn Sie dieses Symbol nicht sehen, wird es möglicherweise ausgeblendet:

1. Wechseln Sie zu **[Einstellungen > Personalisierung > Taskleiste](ms-settings:taskbar?activationSource=GetHelp)**.

2. Klicken Sie im Bereich Benachrichtigung auf **Auswählen, welche Symbole in der Taskleiste angezeigt werden**.

3. Suchen Sie dann das **Power**-Element in der Liste und schalten Sie die Einstellung auf **Ein**.

    ![Power-Symbol in der Taskleiste anzeigen](media/power-icon-on.png)

**Problembehandlung**

Wenn Sie die obigen Anweisungen befolgt haben und der **Power**-Schalter ausgegraut oder nicht sichtbar ist, geben Sie im Suchfeld in der Taskleiste den **Geräte-Manager** ein und wählen Sie dann **Geräte-Manager** in der Ergebnisliste aus. Klicken Sie unter **Akkus** mit der rechten Maustaste auf den Akku für Ihr Gerät, klicken Sie auf **Deaktivieren** und dann auf **Ja**. Warten Sie einige Sekunden, klicken Sie dann mit der rechten Maustaste auf den Akku und klicken Sie auf **Aktivieren**. Starten Sie dann Ihr Gerät neu.

Wenn Sie die obigen Anweisungen befolgt haben, das Akkusymbol jedoch nicht in der Taskleiste angezeigt wird, geben Sie im Suchfeld in der Taskleiste **Task-Manager** ein und klicken Sie dann in der Ergebnisliste auf **Task-Manager**. Klicken Sie mit der rechten Maustaste auf der Registerkarte **Prozesse** unter **Name** auf **Explorer** und klicken Sie dann auf **Neu starten**.
