---
title: Festlegen, dass der Gruppenkalender für Mitglieder schreibgeschützt ist
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3800008"
- "17286"
ms.date: 04/27/2022
ms.openlocfilehash: a8c59338700bb2c50547e95b3db8747376b92a38
ms.sourcegitcommit: b6faebed3da41577a0a16993b065dce49480fa7f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/29/2022
ms.locfileid: "65127243"
---
# <a name="make-the-group-calendar-read-only-for-members"></a>Festlegen, dass der Gruppenkalender für Mitglieder schreibgeschützt ist

Verwenden Sie den folgenden [PowerShell-Befehl](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) :

`Set-UnifiedGroup <groupname> -CalendarMemberReadOnly:$true`

**Hinweise**:

- Ignorieren Sie die Warnmeldung, die am Ende des Befehls angezeigt wird, wenn die Einstellung nicht geändert wurde.
- Die Besitzer der Gruppe können weiterhin Änderungen am Gruppenkalender vornehmen.
- Der Gruppenkalender kann für alle Mitglieder schreibgeschützt gemacht werden, es gibt jedoch keine Möglichkeit, ihn für ausgewählte Mitglieder schreibgeschützt zu machen.

Verwenden Sie den folgenden Befehl, um den Status anzuzeigen:

`Get-UnifiedGroup <groupname> -IncludeAllProperties | fl CalendarMemberReadOnly`
