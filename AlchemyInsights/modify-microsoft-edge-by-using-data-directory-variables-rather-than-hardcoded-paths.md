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
ms.localizationpriority: medium
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: e1247f2547f62fb8a581fe43da31fffb18f1ccce
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63306365"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Ändern Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hartcodierten Pfaden

Legen Sie beispielsweise unter Windows die **UserDataDir** -Richtlinie auf **${local_app_data}\Edge\Profile** fest, um die Profildaten unter den lokalen Anwendungsdaten eines Benutzers und nicht unter dem Standardspeicherort zu speichern. 

Weitere Informationen finden Sie unter [Erstellen Microsoft Edge Benutzerdatenverzeichnisvariablen](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).