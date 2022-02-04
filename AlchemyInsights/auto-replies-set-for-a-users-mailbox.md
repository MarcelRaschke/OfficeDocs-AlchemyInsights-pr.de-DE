---
title: Festlegen von automatischen Antworten für ein Postfach
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: dd14f3228c25c209518b5626d1d4bdf033b88247
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61955146"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Festlegen von automatischen Antworten für das Postfach eines Benutzers

**Methode 1**

1. Melden Sie sich im Microsoft 365-Portal an.

2. Wechseln Sie zu **Benutzer > Aktive Benutzer** (oder **Gruppen > Freigegebene Postfächer**, wenn Sie diese Option für ein freigegebenes Postfach festlegen).

3. Wählen Sie einen Benutzer aus, der über ein Microsoft Exchange-Postfach verfügt.

4. Wechseln Sie im Kontextmenü rechts zu **E-Mail-Einstellungen > Automatische Antworten** (sofern es sich um ein freigegebenes Postfach handelt, klicken Sie einfach auf **Automatische Antworten** im Kontextmenü).

**Methode 2**

1. Melden Sie sich mit Ihren Anmeldeinformationen als Administrator beim Microsoft 365-Verwaltungsportal an.

2. Erweitern Sie **Admin Center**, und klicken Sie auf **Exchange**.

3. Klicken Sie in der oberen rechten Ecke auf das Bild, klicken Sie auf **Ein anderer Benutzer**, und wählen Sie dann das Benutzerpostfach aus, das Sie ändern möchten.

4. Wählen Sie auf der linken Seite **Optionen** aus, klicken Sie auf **E-Mail organisieren**, und klicken Sie dann auf **Automatische Antworten.**

**Methode 3**

Führen Sie das folgenden Cmdlet in Exchange Online PowerShell aus:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Weitere Informationen zu diesem Cmdlet finden Sie unter [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
