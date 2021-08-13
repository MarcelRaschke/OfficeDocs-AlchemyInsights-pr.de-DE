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
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974956"
---
# <a name="move-email-to-the-archive-mailbox"></a>Verschieben von E-Mails in das Archivpostfach

Wenn Sie möchten, dass wir automatisierte Prüfungen für die unten genannten Einstellungen ausführen, wählen Sie die Schaltfläche "Zurück" < - oben auf dieser Seite aus, und geben Sie dann die E-Mail-Adresse des Benutzers ein, der Probleme beim Verschieben von E-Mails in sein Archivpostfach hat.

1. Vergewissern Sie sich, dass ein **Archivpostfach** aktiviert wurde. Wenn nicht, verwenden Sie die Schritte in [diesem Artikel,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) um das Archivpostfach zu aktivieren.

2. Um Nachrichten automatisch im Archivpostfach zu archivieren, muss ein Aufbewahrungstag mit der **Aktion "In Archiv verschieben"** so festgelegt werden, dass es **automatisch auf das gesamte Postfach (Standardtag) angewendet** wird. Führen Sie die hier beschriebenen Schritte aus, um das Tag zu erstellen: [Archivstandardtag.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Fügen Sie als Nächstes der Aufbewahrungsrichtlinie das **Tag "Archiv"** hinzu. Wählen Sie im Exchange Admin Center **Aufbewahrungsrichtlinien** aus, > fügen Sie der Richtlinie das **Tag "In Archiv verschieben"** > **Speichern** hinzu.

4. [Weisen Sie nun die Aufbewahrungsrichtlinie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) dem Postfach des bestimmten Benutzers zu. Die gleiche Richtlinie wird sowohl auf das **Primäre** postfach als auch auf das **Archivpostfach** angewendet.

Es kann erforderlich sein, die Ausführung des Assistenten für verwaltete Ordner (Managed Folder Assistant, MFA) zu erzwingen und die neuen Einstellungen auf das Postfach des Benutzers anzuwenden. Führen Sie den folgenden Befehl aus, während [Sie mit EXO PowerShell verbunden](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sind, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Weitere Informationen zum Einrichten einer Archivrichtlinie finden Sie unter [Einrichten einer Archiv- und Löschrichtlinie für Postfächer.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  