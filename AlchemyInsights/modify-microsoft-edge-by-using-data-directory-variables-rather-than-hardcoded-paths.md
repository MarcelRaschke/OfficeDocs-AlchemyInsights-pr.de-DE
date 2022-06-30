---
title: Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hartcodierten Pfaden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003873"
- "6926"
ms.date: 12/03/2020
ms.openlocfilehash: ca08c44588f8b90da8265c87f4367f044b012329
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66387741"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hartcodierten Pfaden

Legen Sie beispielsweise unter Windows die **UserDataDir** -Richtlinie auf **${local_app_data}\Edge\Profile** fest, um die Profildaten unter den lokalen Anwendungsdaten eines Benutzers und nicht unter dem Standardspeicherort zu speichern. 

Weitere Informationen finden Sie unter [Erstellen von Microsoft Edge-Benutzerdatenverzeichnisvariablen](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).