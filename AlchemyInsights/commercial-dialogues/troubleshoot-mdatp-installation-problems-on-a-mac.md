---
title: Behandeln von MDATP-Installationsproblemen auf einem Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 6d37bdecf65b2dda8f7258d726fddd76d88cd17d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66427387"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Behandeln von MDATP-Installationsproblemen auf einem Mac

Wenn bei der manuellen Installation ein Fehler auftritt, wird auf der **Seite "Zusammenfassung** " des Installations-Assistenten der folgende Fehler angezeigt:

"Während der Installation ist ein Fehler aufgetreten. Fehler beim Installationsprogramm, der dazu führte, dass die Installation fehlschlug. Wenden Sie sich an den Softwarehersteller, um Hilfe zu erhalten."

Bei MDM-Bereitstellungen wird auf der Seite auch ein allgemeiner Installationsfehler angezeigt.

Obwohl endbenutzern keine genauen Fehler angezeigt werden, behalten wir eine Protokolldatei mit dem Installationsfortschritt unter **"/Library/Logs/Microsoft/mdatp/install.log**" bei. Jede Installationssitzung wird an diese Protokolldatei angefügt. Um nur die letzte Installationssitzung auszugeben, verwenden Sie `sed`.

Weitere Informationen finden Sie [unter Beheben von Installationsproblemen für Microsoft Defender ATP für Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
