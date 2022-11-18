---
title: Öffentliche Ordner ausblenden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3500007"
- "8417"
ms.date: 02/18/2021
ms.openlocfilehash: 52accef7918cd222df1f4eb6b493a9219e4d7d7b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66268480"
---
# <a name="hide-public-folders"></a>Öffentliche Ordner ausblenden

**So blenden Sie die gesamte öffentliche Ordnerstruktur aus**:

Verwenden Sie die Schritte in [diesem](https://aka.ms/ControlPF) Artikel, um die gesamte öffentliche Ordnerstruktur vor ausgewählten oder allen Benutzern zu verbergen.

**So blenden Sie einen bestimmten öffentlichen Ordner aus**:

1. Hinzufügen von Berechtigungen für Benutzer, die auf den öffentlichen Ordner zugreifen müssen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Entfernen Sie den Benutzer **Standard** aus der **Berechtigungsliste**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
