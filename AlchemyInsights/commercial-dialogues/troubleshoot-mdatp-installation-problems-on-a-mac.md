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
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 03ec14ac578c17a2405878d2d23ffe9014dff2ce
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63278333"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Behandeln von MDATP-Installationsproblemen auf einem Mac

Wenn die manuelle Installation fehlschlägt, wird auf der Seite **"Zusammenfassung** " des Installations-Assistenten der folgende Fehler angezeigt:

"Während der Installation ist ein Fehler aufgetreten. Beim Installationsprogramm ist ein Fehler aufgetreten, der zu einem Fehler bei der Installation geführt hat. Wenden Sie sich an den Softwarehersteller, um Unterstützung zu erhalten."

Bei MDM-Bereitstellungen wird auf der Seite auch ein allgemeiner Installationsfehler angezeigt.

Obwohl endbenutzern keine genauen Fehler angezeigt werden, behalten wir eine Protokolldatei mit Installationsfortschritt in **"/Library/Logs/Microsoft/mdatp/install.log**" bei. Jede Installationssitzung wird an diese Protokolldatei angefügt. Um nur die letzte Installationssitzung auszugeben, verwenden Sie `sed`.

Weitere Informationen finden Sie unter [Behandeln von Installationsproblemen für Microsoft Defender ATP für Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
