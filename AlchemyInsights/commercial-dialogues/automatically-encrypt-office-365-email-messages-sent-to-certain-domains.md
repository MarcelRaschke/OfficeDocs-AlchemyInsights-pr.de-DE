---
title: Automatische Verschlüsselung Office 365 E-Mail-Nachrichten, die an bestimmte Domänen gesendet werden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 383e5a5cacc411b06f66bc6bc32cf071238ae3df
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62642280"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatische Verschlüsselung Office 365 E-Mail-Nachrichten, die an bestimmte Domänen gesendet werden

1. Wählen Sie im [Exchange Admin Center](https://outlook.office365.com/ecp/) den **Nachrichtenfluss > Regeln** aus. 
2. Klicken Sie auf das Symbol **"Neu" (+),** und klicken Sie dann auf **"Apply Office 365-Nachrichtenverschlüsselung und Rechteschutz für Nachrichten**".
3. Geben Sie in **"Name**" einen Namen für die Regel ein, z. B. *an contoso.com gesendete Nachrichten verschlüsseln*.
4. Wählen **Sie unter "Diese Regel anwenden, wenn****" den Empfänger > Domäne ist**. 
5. Geben Sie den Namen der Domäne ein, z. **B. contoso.com**.
6. Klicken Sie auf das Symbol **"Hinzufügen" (+),** und klicken Sie dann auf **"OK**".
7. Next to the **Do the following** field, click **Select one**. 
8. Wählen Sie im Dropdownmenü der **RMS-Vorlage** **"Verschlüsseln**" aus, und klicken Sie dann auf **"OK**". (Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst. Aber Sie können es hinzufügen!)
9. Wählen Sie eine beliebige optionale Auswahl aus (aus einer Liste optionaler Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber mit der Standardeinstellung übrig bleiben können).
10. Klicken Sie auf **Speichern**.

**Wichtig**: Sie können jederzeit zurückkehren und diese Regel später bearbeiten.

Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)