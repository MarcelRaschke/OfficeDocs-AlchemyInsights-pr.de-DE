---
title: Fehlender oder ungenauer Softwarebestand
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: 66c79af81301ef6478b9be23a1a5b97583d4781f
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61989267"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Fehlender oder ungenauer Softwarebestand

Der Softwarebestand in der Bedrohungs- und Sicherheitsrisikoverwaltung (TVM) ist eine Liste bekannter Software in Ihrer Organisation mit offiziellen CPEs (Common Platform Enumerations).

Für Softwareprodukte ohne offizielle CPE wurde keine Sicherheitsrisiken veröffentlicht. Der Bestand umfasst auch Details wie den Namen des Anbieters, die Anzahl der Schwachstellen, Bedrohungen sowie die Anzahl der gefährdeten Geräte.

Softwareänderungen auf Geräten werden in der Regel innerhalb von zwei Stunden in Sicherheitsportalen widergespiegelt. Es kann jedoch manchmal länger dauern. Derzeit gibt es keine Möglichkeit, eine Synchronisierung zu erzwingen. Es handelt sich um eine kontinuierliche Bewertung.

Wenn Sie eine Softwareänderung vorgenommen haben und die Änderung nach 5 Stunden in TVM nicht präzise widergespiegelt wird, führen Sie die folgenden Schritte aus:

1. Überprüfen Sie den Abschnitt „Softwarenachweis“, um zu verstehen, wie die Software erkannt wurde.
1. Stellen Sie sicher, dass die Software unterstützt wird. Software ist möglicherweise nur auf Geräteebene sichtbar, auch wenn sie aktuell nicht von der Bedrohungs- und Sicherheitsrisikoverwaltung unterstützt wird. Es stehen jedoch nur eingeschränkte Daten zur Verfügung.
1. Schritte, wie Sie Ungenauigkeiten im Portal melden können, finden Sie unter [Ungenauigkeit melden](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-software-inventory#report-inaccuracy).
   
    **Hinweis**: Das Melden einer Ungenauigkeit über das MDE-Portal ist ein Einwegkanal für Techniker. Wenn das Problem dringend ist, öffnen Sie ein Supportticket.

Weitere Informationen finden Sie unter [Softwarebestand – Bedrohungs- und Sicherheitsrisikoverwaltung](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-software-inventory).