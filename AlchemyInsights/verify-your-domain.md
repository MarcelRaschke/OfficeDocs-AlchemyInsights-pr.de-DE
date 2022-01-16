---
title: Verify your domain
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 8da12202b8524e7ae56d3107256005a9994077f6
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61981931"
---
# <a name="verify-your-domain"></a>Verify your domain

 **Der Datensatz wurde wahrscheinlich nicht über das Internet aktualisiert.**
  
In der Regel dauert es nur ein paar Minuten, bis wir den neuen Eintrag sehen können, aber gelegentlich kann es auch ein paar Stunden dauern. 
  
- If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. Ein häufiges Problem ist, dass der Teil "MS=" des Eintrags fehlt. Diese Angabe ist ebenfalls erforderlich!

- Bei einigen DNS-Hosts müssen Sie einen zusätzlichen Schritt ausführen, um die Zonendatei zu speichern (in der der DNS-Eintrag gespeichert ist), damit der Eintrag im Internet aktualisiert wird. Stellen Sie sicher, dass Sie Ihre Änderungen gespeichert haben, damit Microsoft den Datensatz sehen und überprüfen kann.
