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
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945741"
---
# <a name="hide-public-folders"></a>Öffentliche Ordner ausblenden

**So blenden Sie die gesamte öffentliche Ordnerstruktur aus**:

Verwenden Sie die Schritte in [diesem](https://aka.ms/ControlPF) Artikel, um die gesamte öffentliche Ordnerstruktur vor ausgewählten oder allen Benutzern zu verbergen.

**So blenden Sie einen bestimmten öffentlichen Ordner aus**:

1. Hinzufügen von Berechtigungen für Benutzer, die auf den öffentlichen Ordner zugreifen müssen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Entfernen Sie den Benutzer **Standard** aus der **Berechtigungsliste**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
