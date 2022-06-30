---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e4f4c17b4d5cd47c6e3e4b52b96b1e3946ed322e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66301348"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Beheben von Übermittlungsproblemen für Fehlercode 550 5.4.1 Relayzugriff verweigert

Dieses Problem tritt auf, wenn [überprüft wird, ob eine E-Mail-Adresse gültig ist, um Rücksprünge beim Betreten des Microsoft-Netzwerks zu verhindern](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) . Versuchen Sie, das Problem durch folgende Maßnahme zu beheben:

1. Ermitteln Sie, ob das Problem für eine gesamte Domäne oder eine einzelne E-Mail-Adresse spezifisch ist:
    - Ganze Domäne: Manchmal muss die Domäne synchronisiert werden; Versuchen Sie [, die Domäne auf "Intern" und dann wieder auf "Autoritativ" festzulegen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Einzelne E-Mail-Adresse: Manchmal muss die Adresse synchronisiert werden; Das Ändern der SMTP-Proxyadresse und das anschließende Zurückwechseln kann hilfreich sein.
2. Ermitteln Sie, ob das Problem für eine Gruppe oder einen öffentlichen Ordner spezifisch ist. Bei einigen Objekttypen müssen die Objekte möglicherweise manuell in Azure Active Directory erstellt werden.

Wenn Sie zusätzliche Hilfe benötigen, öffnen Sie bitte ein Supportticket, und geben Sie den Umfang des Problems an (einschließlich des Typs des Objekts, an das Sie senden), damit wir Ihnen besser helfen können.