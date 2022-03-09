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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 4819458183c39ed6e814af463c65c2cd9797ff7c
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63295942"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Ändern von Microsoft Edge mithilfe von Datenverzeichnisvariablen anstelle von hart codierten Pfaden

Legen Sie beispielsweise unter Windows die *UserDataDir* -Richtlinie auf **${local_app_data}\Edge\Profile** fest, um die Profildaten unter den lokalen Anwendungsdaten eines Benutzers und nicht unter dem Standardspeicherort zu speichern.

Weitere Informationen finden Sie unter [Erstellen von Microsoft Edge-Benutzerdatenverzeichnisvariablen](https://docs.microsoft.com/deployedge/microsoft-edge-policies).