---
title: Der Besitzer kann keinen öffentlichen Ordner löschen.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "18180"
ms.openlocfilehash: 1466ae29f7e4fcab4f7a7ab48fc3a44c47d209b4
ms.sourcegitcommit: 7c650f8e0593bbb15db359384b89550a35ab7707
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2022
ms.locfileid: "67571946"
---
# <a name="owner-cannot-delete-public-folder"></a>Der Besitzer kann keinen öffentlichen Ordner löschen.

Benutzer mit entsprechenden Berechtigungen, die keine öffentlichen Ordner aus Outlook löschen können, können Folgendes ausprobieren:

- Der öffentliche Ordner, der gelöscht wird, ist E-Mail aktiviert. Weitere Informationen finden Sie [unter Fehler beim Löschen eines öffentlichen Ordners aus Outlook-Clients](https://docs.microsoft.com/exchange/troubleshoot/public-folders/cannot-delete-public-folder).

- Das primäre Postfach für öffentliche Ordner der Hierarchie für den betroffenen Benutzer ist "DefaultPublicFolderMailbox/EffectivePublicFolderMailbox". Wenn ja, verwenden Sie eine der folgenden Problemumgehungen:

    - Verwenden Sie diesen [EXO PowerShell-Befehl](https://aka.ms/EXOPowerShellV2) , um dem Benutzer, der den öffentlichen Ordner löschen muss, ein Sekundärhierarchiepostfach für öffentliche Ordner als DefaultPublicFolderMailbox zuzuweisen:
    
    `Set-Mailbox <username> -DefaultPublicFolderMailbox <name_of_secondary_hierarchy_PF_mailbox>`

    **Hinweis**: Die Änderung in "Default/EffectivePublicFolderMailbox" dauert bis zu einer Stunde, bis sie auf dem Client widerzuspiegeln ist.

- Der Mandantenadministrator kann den gewünschten öffentlichen Ordner aus [EXO PowerShell](https://aka.ms/EXOPowerShellV2) löschen.