---
title: Warnungen fehlen auf der Registerkarte "Warnungen"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: e2047d0eb0caf4c4c9c89053f8b8ed9f3d725e9a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63095050"
---
# <a name="alerts-missing-from-alerts-tab"></a>Warnungen fehlen auf der Registerkarte "Warnungen"

Die Registerkarte **"Warnungen** " funktioniert basierend auf den Setup- und aktivierten Richtlinien des App-Governance-Portals in Ihrem Mandanten. Out-of-the-Box-Richtlinien in App Governance müssen ebenfalls aktiviert werden, damit Signale zur Registerkarte **"Warnungen** " fließen können. 

Vergewissern Sie sich, dass die Warnung generiert wurde:

1. Wechseln Sie zu [App-Governancerichtlinien](https://compliance.microsoft.com/m365appprotection?viewid=policies) , und bestätigen Sie, dass Sie mindestens eine aktive oder Überwachungsrichtlinie erstellt haben.

1. Wählen Sie die Richtlinie aus, und wählen Sie dann im Flyoutbereich " **Bearbeiten** " aus. 

1. Überprüfen Sie die Richtlinienkonfiguration, um zu überprüfen, ob eine Warnung basierend auf einem Richtlinienereignis generiert worden sein sollte, das vor mehr als 24 Stunden initiiert wurde.

Weitere Informationen zu Warnungen in App Governance finden Sie unter ["Erste Schritte mit der Erkennung und Behebung von App-Bedrohungen](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)".