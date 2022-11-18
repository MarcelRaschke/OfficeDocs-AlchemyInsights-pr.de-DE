---
title: S/MIME in Outlook im Web
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 9000329
ms.openlocfilehash: e82aafc9de4d8c5565fed8e44339bd740a2b30f1
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66518988"
---
# <a name="encrypt-email-messages-in-outlook"></a>Verschlüsseln von E-Mail-Nachrichten in Outlook

Die Microsoft 365-Nachrichtenverschlüsselung basiert auf Microsoft Azure Rights Management (Azure RMS), das Teil von Azure Information Protection ist. Wenn Ihr Abonnement Azure Rights Management oder Azure Information Protection umfasst, **müssen Sie keine Maßnahmen ergreifen, um den Rights Management Service manuell zu aktivieren oder zu aktivieren**.

Basierend auf kundenbezogenem Feedback aktivieren wir exchange-Nachrichtenflussregeln nicht mehr, um ausgehende E-Mails, die bestimmte Arten vertraulicher Informationen in Ihrem Mandanten enthalten, standardmäßig automatisch zu verschlüsseln. Stattdessen geben wir Ihnen detaillierte Anweisungen, wie Sie dies selbst tun können. Weitere Informationen zum Erstellen einer Transportregel zum Verschlüsseln vertraulicher Informationen finden Sie [in diesem Artikel](https://aka.ms/OmeEtr).

- Wenn Sie Outlook im Web (früher **OWA**) verwenden: Klicken Sie beim Verfassen einer E-Mail-Nachricht einfach in OWA auf **"Schützen** ". Dies gilt für die Berechtigung "Nicht weiterleiten". Klicken Sie auf **"Berechtigung ändern"** , und wählen Sie " **Verschlüsseln** " aus, um die Nachricht nur zu verschlüsseln.

- Wenn **Sie den Outlook-Client** verwenden: Um eine verschlüsselte Nachricht aus Outlook 2013 oder 2016 oder Outlook 2016 für Mac zu senden, wählen Sie **"Optionsberechtigungen** > " und dann die gewünschte Schutzoption aus.

- Um alle an bestimmte Empfänger oder externe Partnerorganisationen gesendeten **E-Mails automatisch zu verschlüsseln** , müssen Sie im Exchange Admin Center eine Nachrichtenfluss-Transportregel erstellen. Ausführliche Anweisungen finden Sie in [diesem Supportartikel](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

