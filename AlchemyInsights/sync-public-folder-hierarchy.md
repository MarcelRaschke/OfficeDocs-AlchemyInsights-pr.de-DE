---
title: Öffentliche Ordnerhierarchie synchronisieren
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
- "16396"
ms.date: 01/21/2022
ms.openlocfilehash: 7229443bcc20e0a80e0e625932bc1a5178f493a2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66315327"
---
# <a name="sync-public-folder-hierarchy"></a>Öffentliche Ordnerhierarchie synchronisieren

Es konnten Probleme wie der öffentliche Ordner angezeigt werden, die für bestimmte Benutzer oder Benutzer nicht in der Lage sind, eine Aktion auszuführen, obwohl sie über den richtigen Zugriff auf Rechte verfügen. Dies sind Indikatoren, die die Hierarchie öffentlicher Ordner nicht synchronisiert.

Führen Sie den folgenden Befehl aus, um eine Hierarchiesynchronisierung zu erzwingen:

`Update-PublicFolderMailbox <PFMailboxName> -InvokeSynchronizer`

Weitere Informationen finden Sie [unter Einführung in die Synchronisierung der Hierarchie öffentlicher Ordner](https://aka.ms/PFHierarchy).
