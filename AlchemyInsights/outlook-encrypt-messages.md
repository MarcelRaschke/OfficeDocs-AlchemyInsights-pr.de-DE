---
title: S/MIME in Outlook im Web
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 8e4cd213f1b2fd89f1a0eab694d6212775da4ea3
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61947238"
---
# <a name="encrypt-email-messages-in-outlook"></a>Verschlüsseln von E-Mail-Nachrichten in Outlook

Microsoft 365 Nachrichtenverschlüsselung basiert auf Microsoft Azure Rights Management (Azure RMS), das Teil von Azure Information Protection ist. Wenn Ihr Abonnement Azure Rights Management oder Azure Information Protection umfasst, müssen Sie keine Maßnahmen ergreifen, um den Rights Management Service **manuell zu aktivieren oder zu aktivieren.**

Basierend auf dem Kundenfeedback aktivieren wir Exchange Nachrichtenflussregeln nicht mehr, um ausgehende E-Mails mit bestimmten vertraulichen Informationen in Ihrem Mandanten standardmäßig automatisch zu verschlüsseln. Stattdessen stellen wir detaillierte Anweisungen dazu bereit, wie Sie dies tun können. Weitere Informationen zum Erstellen einer Transportregel zum Verschlüsseln vertraulicher Informationen finden Sie in [diesem Artikel.](https://aka.ms/OmeEtr)

- Wenn Sie Outlook im Web (früher **OWA)** verwenden: Klicken Sie beim Verfassen einer E-Mail-Nachricht einfach auf **"Schützen"** in OWA. Dies gilt für die Berechtigung "Nicht weiterleiten". Klicken Sie auf **"Berechtigung ändern",** und wählen Sie **"Verschlüsseln"** aus, um die Nachricht nur zu verschlüsseln.

- Wenn **Sie Outlook Client** verwenden: Um eine verschlüsselte Nachricht aus Outlook 2013 oder 2016 oder Outlook 2016 für Mac zu senden, wählen Sie   >  **Optionenberechtigungen** und dann die gewünschte Schutzoption aus.

- Um **alle E-Mails,** die an bestimmte Empfänger oder externe Partnerorganisationen gesendet werden, automatisch zu verschlüsseln, müssen Sie im Exchange Admin Center eine Nachrichtenfluss-Transportregel erstellen. Ausführliche Anweisungen finden Sie in [diesem Supportartikel.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

