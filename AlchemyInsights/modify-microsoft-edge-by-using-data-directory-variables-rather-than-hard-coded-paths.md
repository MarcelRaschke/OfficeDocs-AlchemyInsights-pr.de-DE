---
title: Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hart codierten Pfaden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: ba227b8e29b81420bce187844edaf0cc40639fd9
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62666635"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hart codierten Pfaden

Legen Sie beispielsweise unter Windows die *UserDataDir* -Richtlinie auf **${local_app_data}\Edge\Profile** fest, um die Profildaten unter den lokalen Anwendungsdaten eines Benutzers und nicht unter dem Standardspeicherort zu speichern.

Weitere Informationen finden Sie unter [Erstellen von Microsoft Edge-Benutzerdatenverzeichnisvariablen](https://docs.microsoft.com/deployedge/microsoft-edge-policies).