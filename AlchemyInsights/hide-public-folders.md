---
title: Öffentliche Ordner ausblenden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: d9b209ff3e50531fc86385eff46b4a4c55267c1b
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62576271"
---
# <a name="hide-public-folders"></a>Öffentliche Ordner ausblenden

**So blenden Sie die gesamte öffentliche Ordnerstruktur aus**:

Verwenden Sie die Schritte in [diesem](https://aka.ms/ControlPF) Artikel, um die gesamte öffentliche Ordnerstruktur vor ausgewählten oder allen Benutzern zu verbergen.

**So blenden Sie einen bestimmten öffentlichen Ordner aus**:

1. Hinzufügen von Berechtigungen für Benutzer, die auf den öffentlichen Ordner zugreifen müssen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Entfernen Sie den Benutzer **Standard** aus der **Berechtigungsliste**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
