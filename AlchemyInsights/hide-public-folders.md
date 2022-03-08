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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: f3a05dc589f8e314f3aa7c251059bf5673ae6526
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63128549"
---
# <a name="hide-public-folders"></a>Öffentliche Ordner ausblenden

**So blenden Sie die gesamte öffentliche Ordnerstruktur aus**:

Verwenden Sie die Schritte in [diesem](https://aka.ms/ControlPF) Artikel, um die gesamte öffentliche Ordnerstruktur vor ausgewählten oder allen Benutzern zu verbergen.

**So blenden Sie einen bestimmten öffentlichen Ordner aus**:

1. Hinzufügen von Berechtigungen für Benutzer, die auf den öffentlichen Ordner zugreifen müssen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Entfernen Sie den Benutzer **Standard** aus der **Berechtigungsliste**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
