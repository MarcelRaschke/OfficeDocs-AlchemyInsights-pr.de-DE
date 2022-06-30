---
title: Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hart codierten Pfaden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004596"
- "8222"
ms.date: 03/19/2021
ms.openlocfilehash: a17f8ce521f103a9a63c7d79fb32bce2526b32a6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66402627"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hart codierten Pfaden

Legen Sie beispielsweise unter Windows die *UserDataDir* -Richtlinie auf **${local_app_data}\Edge\Profile** fest, um die Profildaten unter den lokalen Anwendungsdaten eines Benutzers und nicht unter dem Standardspeicherort zu speichern.

Weitere Informationen finden Sie unter [Erstellen von Microsoft Edge-Benutzerdatenverzeichnisvariablen](https://docs.microsoft.com/deployedge/microsoft-edge-policies).