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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: a7af19f281ba6bae9425f9acd4fee2bae7ea1ce7
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61947491"
---
# <a name="alerts-missing-from-alerts-tab"></a>Warnungen fehlen auf der Registerkarte "Warnungen"

Die Registerkarte **"Warnungen"** funktioniert basierend auf den Setup- und aktivierten Richtlinien des App-Governance-Portals in Ihrem Mandanten. Out-of-the-Box-Richtlinien in App Governance müssen ebenfalls aktiviert werden, damit Signale zur Registerkarte **"Warnungen"** fließen können. 

Vergewissern Sie sich, dass die Warnung generiert wurde:

1. Wechseln Sie zu [App-Governancerichtlinien,](https://compliance.microsoft.com/m365appprotection?viewid=policies) und bestätigen Sie, dass Sie mindestens eine aktive oder Überwachungsrichtlinie erstellt haben.

1. Wählen Sie die Richtlinie aus, und wählen Sie dann im Flyoutbereich **"Bearbeiten"** aus. 

1. Überprüfen Sie die Richtlinienkonfiguration, um zu überprüfen, ob eine Warnung basierend auf einem Richtlinienereignis generiert worden sein sollte, das vor mehr als 24 Stunden initiiert wurde.

Weitere Informationen zu Warnungen in App Governance finden Sie unter "Erste Schritte mit der Erkennung und Behebung von [App-Bedrohungen".](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)