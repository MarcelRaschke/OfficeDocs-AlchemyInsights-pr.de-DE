---
title: Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003388"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten

**Symptom**

Benutzer können keine Berichte öffnen. "Es ist ein Fehler aufgetreten. Überprüfen Sie die technischen Details, um weitere Informationen zu erhalten."

**Ursache**

Berichte können nicht in UCI geladen werden, und der Fehler "Formularbeschreibung ist "null" oder nicht definiert" wird angezeigt. Berichte in UCI erfordern immer noch alte Dialoge, daher muss im System des Kunden *allowlegacydialogsembedding* aktiviert sein.

**Lösung**

1. Navigieren Sie zu **Einstellungen > Verwaltung > Systemeinstellungen > Registerkarte "Allgemein"**.

2. Legen Sie "Einbettung bestimmter alter Dialoge in den Browserclient der einheitlichen Oberfläche aktivieren" auf **Ja** fest.
