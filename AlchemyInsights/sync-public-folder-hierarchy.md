---
title: Synchronisieren der Hierarchie öffentlicher Ordner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "16396"
ms.date: 01/21/2022
ms.openlocfilehash: 96b23723be2910e9a623769fcded83d60c5d3884
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63179203"
---
# <a name="sync-public-folder-hierarchy"></a>Synchronisieren der Hierarchie öffentlicher Ordner

Es könnten Probleme auftreten, z. B. dass der öffentliche Ordner für bestimmte Benutzer nicht angezeigt wird oder dass Benutzer trotz korrekten Zugriffsrechten keine Aktion ausführen können. Dies sind Indikatoren, die zeigen, dass die Hierarchie öffentlicher Ordner nicht synchronisiert ist.

Führen Sie den folgenden Befehl aus, um eine Hierarchiesynchronisierung zu erzwingen:

`Update-PublicFolderMailbox <PFMailboxName> -InvokeSynchronizer`

Weitere Informationen finden Sie unter ["Einführung in die Synchronisierung der Hierarchie öffentlicher Ordner"](https://aka.ms/PFHierarchy).
