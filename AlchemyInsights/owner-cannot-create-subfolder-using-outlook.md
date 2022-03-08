---
title: Besitzer kann keinen Unterordner mit Outlook erstellen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 91e678547ba38c9c7e43ae89dfbdcf77b2b4418d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63271133"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Besitzer kann keinen Unterordner mit Outlook erstellen

**Es gibt ein anhaltendes Problem mit Besitzern öffentlicher Ordner, die Unterordner mit Outlook erstellen. Das Problem wird in Kürze behoben.**

In der Zwischenzeit können Sie eine der folgenden Problemumgehungen verwenden:

1. Verwenden Sie Outlook für MAC, um den Unterordner zu erstellen, da das Problem nur Outlook für Desktop-Fenster betrifft (alle Versionen)
2. Lassen Sie den Administrator den Unterordner mit EXO Shell oder EAC erstellen
3. Ändern von DefaultPublicFolderMailbox/EffectivePublicFolderMailbox des Benutzers in ein anderes Postfach als das Inhaltspostfach für den Ordner, der das Problem verursacht  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Warten Sie eine Stunde, und starten Sie den Outlook-Client erneut