---
title: Verschieben von E-Mail-Nachrichten in das Archivpostfach
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: cfbafc1b07f37228eac30c6b295657fc82d44162
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63191444"
---
# <a name="move-email-to-the-archive-mailbox"></a>Verschieben von E-Mails in das Archivpostfach

Wenn Sie möchten, dass wir automatisierte Überprüfungen für die unten genannten Einstellungen ausführen, wählen Sie die Schaltfläche "Zurück" < aus – oben auf dieser Seite, und geben Sie dann die E-Mail-Adresse des Benutzers ein, der Probleme beim Verschieben von E-Mails in sein Archivpostfach hat.

1. Vergewissern Sie sich, dass ein **Archivpostfach** aktiviert wurde. Wenn nicht, verwenden Sie die Schritte in [diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , um das Archivpostfach zu aktivieren.

2. Um Nachrichten automatisch im Archivpostfach zu archivieren, muss ein Aufbewahrungstag mit der **Aktion "In Archiv verschieben** " so festgelegt werden, dass es **automatisch auf das gesamte Postfach (Standardtag) angewendet** wird. Führen Sie die hier beschriebenen Schritte aus, um das Tag zu erstellen: [Archivstandardtag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Fügen Sie als Nächstes der Aufbewahrungsrichtlinie das **Tag "Archiv"** hinzu. Wählen Sie im Exchange Admin Center **Aufbewahrungsrichtlinien** aus, > fügen Sie das **Tag "In Archiv verschieben**" zur Richtlinie > **Speichern** hinzu.

4. [Weisen Sie nun die Aufbewahrungsrichtlinie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) dem Postfach des bestimmten Benutzers zu. Die gleiche Richtlinie wird sowohl auf das **Primäre** postfach als auch auf das **Archivpostfach** angewendet.

Es kann erforderlich sein, die Ausführung des Assistenten für verwaltete Ordner (Managed Folder Assistant, MFA) zu erzwingen und die neuen Einstellungen auf das Postfach des Benutzers anzuwenden. Führen Sie den folgenden Befehl aus, während [Sie mit EXO PowerShell verbunden](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) sind, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:
  
`Start-ManagedFolderAssistant -Identity <name of the mailbox>`

Weitere Informationen zum Einrichten einer Archivrichtlinie finden Sie unter ["Einrichten einer Archivierungs- und Löschrichtlinie für Postfächer"](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  