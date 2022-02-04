---
title: Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
  - 9002931
  - 5612
---

# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten

**Symptom**

Benutzer können keine Berichte öffnen. "Es ist ein Fehler aufgetreten. Überprüfen Sie die technischen Details, um weitere Informationen zu erhalten."

**Ursache**

Berichte können nicht in UCI geladen werden, und der Fehler "Formularbeschreibung ist "null" oder nicht definiert" wird angezeigt. Berichte in UCI erfordern immer noch alte Dialoge, daher muss im System des Kunden *allowlegacydialogsembedding* aktiviert sein.

**Lösung**

1. Navigieren Sie zu **Einstellungen > Verwaltung > Systemeinstellungen > Registerkarte "Allgemein"**.

2. Legen Sie "Einbettung bestimmter alter Dialoge in den Browserclient der einheitlichen Oberfläche aktivieren" auf **Ja** fest.
