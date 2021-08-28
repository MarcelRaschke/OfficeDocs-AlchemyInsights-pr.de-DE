---
title: Kalenderereignisse fehlen oder werden nicht aktualisiert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: af45345bc8779489f5e00dcaee136103e674068e29c77d8c536d012f475c33c5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968698"
---
# <a name="calendar-events-missing-or-not-updating"></a>Kalenderereignisse fehlen oder werden nicht aktualisiert

Wenn Kalenderelemente fehlen oder nicht aktualisiert werden, beginnen Sie mit der Überprüfung der Elementanzahl in den Eigenschaften Ihres Kalenderordners in Outlook: 

1. Klicken Sie mit der rechten Maustaste auf den betroffenen Benutzer-**Kalenderordner** und dann auf **Eigenschaften**.

1. Wählen Sie die Registerkarte **Synchronisierung** aus.

Wenn die Elementanzahl im Serverordner nicht die gleiche wie die im Offlineordner ist:

1.  Markieren Sie den **Kalenderordner**.

1.  Wechseln Sie zur Registerkarte **Senden**/**Empfangen**, und klicken Sie dann auf **Ordner aktualisieren**.

Wenn Ihr Kalender immer noch nicht aktualisiert wird oder Ereignisse fehlen, laden Sie das Tool für die Kalenderüberprüfung für Outlook aus dem [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=28786) herunter. Überprüfen Sie, ob der Kalenderordner mehr als 5.000 Elemente enthält, da dies zu Symptomen wie nicht aktualisierten Kalenderbesprechungen oder Besprechungsfehlern führen kann. 

Weitere Informationen finden Sie unter [Outlook-Leistungsprobleme bei zu vielen Elementen oder Ordnern in einer OST- oder PST-Datei im Cachemodus](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).