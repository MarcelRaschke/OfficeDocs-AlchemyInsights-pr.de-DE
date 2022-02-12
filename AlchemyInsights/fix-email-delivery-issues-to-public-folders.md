---
title: Beheben von Problemen bei der E-Mail-Zustellung an E-Mail-aktivierte öffentliche Ordner
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
- "1956"
- "3500007"
ms.openlocfilehash: 808db6cf6808eb76e5ca094f4f779b3add8123f4
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62757611"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Beheben von Problemen bei der E-Mail-Zustellung an E-Mail-aktivierte öffentliche Ordner

Wenn externe Absender keine Nachrichten an Ihre E-Mail-aktivierten öffentlichen Ordner senden können und die Absender den Fehler erhalten: **Konnte nicht gefunden werden (550 5.4.1),** überprüfen Sie, ob die E-Mail-Domäne für den öffentlichen Ordner als interne Relaydomäne anstelle einer autorisierenden Domäne konfiguriert ist:

1. Öffnen Sie das [Exchange Admin Center (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Wechseln Sie zum **Nachrichtenfluss** \> **"Akzeptierte Domänen**", wählen Sie die akzeptierte Domäne aus, und klicken Sie dann auf **"Bearbeiten**".

3. Wenn der Domänentyp auf **"Autoritativ"** festgelegt ist, ändern Sie auf der daraufhin geöffneten Eigenschaftenseite den Wert in **"Internes Relay** ", und klicken Sie dann auf **"Speichern**".

Wenn externe Absender den Fehler erhalten **, dass Sie nicht über die Berechtigung verfügen (550 5.7.13),** führen Sie den folgenden Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aus, um die Berechtigungen für anonyme Benutzer im öffentlichen Ordner anzuzeigen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Beispiel: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Damit externe Benutzer E-Mails an diesen öffentlichen Ordner senden können, fügen Sie dem Benutzer "Anonym" das Zugriffsrecht "CreateItems" hinzu. Beispiel: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
