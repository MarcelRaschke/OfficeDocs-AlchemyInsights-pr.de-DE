---
title: Besitzer kann keinen Unterordner mit Outlook erstellen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3500007"
- "5884"
ms.date: 04/21/2020
ms.openlocfilehash: 20ba3757ffd0c47ad6eb7cd0f54569359b2e1521
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66305874"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Besitzer kann keinen Unterordner mit Outlook erstellen

**Es gibt ein anhaltendes Problem mit Besitzern öffentlicher Ordner, die Unterordner mit Outlook erstellen. Das Problem wird in Kürze behoben.**

In der Zwischenzeit können Sie eine der folgenden Problemumgehungen verwenden:

1. Verwenden Sie Outlook für MAC, um den Unterordner zu erstellen, da das Problem nur Outlook für Desktop-Fenster betrifft (alle Versionen)
2. Lassen Sie den Administrator den Unterordner mit EXO Shell oder EAC erstellen
3. Ändern von DefaultPublicFolderMailbox/EffectivePublicFolderMailbox des Benutzers in ein anderes Postfach als das Inhaltspostfach für den Ordner, der das Problem verursacht  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Warten Sie eine Stunde, und starten Sie den Outlook-Client erneut