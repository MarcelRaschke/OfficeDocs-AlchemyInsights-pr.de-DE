---
title: Warnungen fehlen auf der Registerkarte "Warnungen"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: f1b676d155f0f6aa87ade418fee8470af9f73fdf
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66302490"
---
# <a name="alerts-missing-from-alerts-tab"></a>Warnungen fehlen auf der Registerkarte "Warnungen"

Die Registerkarte **"Warnungen** " basiert auf den Setup- und aktivierten Richtlinien aus dem App-Governance-Portal in Ihrem Mandanten. Out-of-the-Box-Richtlinien in App Governance müssen auch aktiviert werden, damit Signale zur Registerkarte **"Warnungen** " fließen können. 

Vergewissern Sie sich, dass die Warnung generiert wurde:

1. Wechseln Sie zu [App-Governancerichtlinien](https://compliance.microsoft.com/m365appprotection?viewid=policies) , und vergewissern Sie sich, dass Sie mindestens eine aktive oder Überwachungsrichtlinie erstellt haben.

1. Wählen Sie die Richtlinie aus, und wählen Sie dann " **Bearbeiten"** im Flyoutbereich aus. 

1. Überprüfen Sie die Richtlinienkonfiguration, um zu bestätigen, dass eine Warnung basierend auf einem Richtlinienereignis generiert werden sollte, das vor mehr als 24 Stunden initiiert wurde.

Weitere Informationen zu Warnungen in App-Governance finden [Sie unter "Erste Schritte mit der Erkennung und Behebung von App-Bedrohungen](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)".