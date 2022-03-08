---
title: Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: cffd210240f6f6698688d5a02e3b1e5284cc21c5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63247985"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten

**Symptom**

Benutzer können keine Berichte öffnen. "Es ist ein Fehler aufgetreten. Überprüfen Sie die technischen Details, um weitere Informationen zu erhalten."

**Ursache**

Berichte können nicht in UCI geladen werden, und der Fehler "Formularbeschreibung ist "null" oder nicht definiert" wird angezeigt. Berichte in UCI erfordern immer noch alte Dialoge, daher muss im System des Kunden *allowlegacydialogsembedding* aktiviert sein.

**Lösung**

1. Navigieren Sie zu **Einstellungen > Verwaltung > Systemeinstellungen > Registerkarte "Allgemein"**.

2. Legen Sie "Einbettung bestimmter alter Dialoge in den Browserclient der einheitlichen Oberfläche aktivieren" auf **Ja** fest.
