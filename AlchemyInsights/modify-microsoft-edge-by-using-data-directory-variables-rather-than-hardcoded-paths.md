---
title: Ändern Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hartcodierten Pfaden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: e71322b065f200d782af207ab5db740244db79c6
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62619744"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Ändern Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hartcodierten Pfaden

Legen Sie beispielsweise unter Windows die **UserDataDir** -Richtlinie auf **${local_app_data}\Edge\Profile** fest, um die Profildaten unter den lokalen Anwendungsdaten eines Benutzers und nicht unter dem Standardspeicherort zu speichern. 

Weitere Informationen finden Sie unter [Erstellen Microsoft Edge Benutzerdatenverzeichnisvariablen](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).