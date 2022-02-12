---
title: Synchronisieren der Hierarchie öffentlicher Ordner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "16396"
ms.date: 01/21/2022
ms.openlocfilehash: 469f4a655b8cdb89d09babf76895a48952c2820d
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62661918"
---
# <a name="sync-public-folder-hierarchy"></a>Synchronisieren der Hierarchie öffentlicher Ordner

Es könnten Probleme auftreten, z. B. dass der öffentliche Ordner für bestimmte Benutzer nicht angezeigt wird oder dass Benutzer trotz korrekten Zugriffsrechten keine Aktion ausführen können. Dies sind Indikatoren, die zeigen, dass die Hierarchie öffentlicher Ordner nicht synchronisiert ist.

Führen Sie den folgenden Befehl aus, um eine Hierarchiesynchronisierung zu erzwingen:

`Update-PublicFolderMailbox <PFMailboxName> -InvokeSynchronizer`

Weitere Informationen finden Sie unter ["Einführung in die Synchronisierung der Hierarchie öffentlicher Ordner"](https://aka.ms/PFHierarchy).
