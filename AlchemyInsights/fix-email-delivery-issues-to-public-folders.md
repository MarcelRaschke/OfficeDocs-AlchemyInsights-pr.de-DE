---
title: Beheben von Problemen mit der Zustellung von E-Mails in E-Mail-aktivierte öffentliche Ordner
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "1956"
ms.date: 04/21/2020
ms.openlocfilehash: 19bd34320a5cd5f2d8dd00f185c936fbe9479d53
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66434920"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Beheben von Problemen mit der Zustellung von E-Mails in E-Mail-aktivierte öffentliche Ordner

Wenn externe Absender keine Nachrichten an Ihre E-Mail-aktivierten öffentlichen Ordner senden können und die Absender die Fehlermeldung erhalten: **Konnte nicht gefunden werden (550 5.4.1)**, überprüfen Sie, ob die E-Mail-Domäne für den öffentlichen Ordner als interne Relaydomäne anstelle einer autorisierenden Domäne konfiguriert ist:

1. Öffnen Sie das [Exchange Admin Center (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Wechseln Sie zu **"Akzeptierte Nachrichtenflussdomänen**\>", wählen Sie die akzeptierte Domäne aus, und klicken Sie dann auf **"Bearbeiten"**.

3. Wenn der Domänentyp auf der daraufhin geöffneten Eigenschaftenseite auf " **Autoritativ**" festgelegt ist, ändern Sie den Wert in **"Internes Relay** ", und klicken Sie dann auf **"Speichern"**.

Wenn externe Absender den Fehler erhalten, dass **Sie nicht berechtigt sind (550 5.7.13),** führen Sie den folgenden Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aus, um die Berechtigungen für anonyme Benutzer im öffentlichen Ordner anzuzeigen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Beispiel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`: .

Damit externe Benutzer E-Mails an diesen öffentlichen Ordner senden können, fügen Sie dem Anonymen Benutzer das CreateItems-Zugriffsrecht hinzu. Beispiel: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
