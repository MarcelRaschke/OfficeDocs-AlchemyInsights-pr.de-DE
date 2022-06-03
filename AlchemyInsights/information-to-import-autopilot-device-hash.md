---
title: Zum Importieren des Autopilot-Gerätehashs erforderliche Informationen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "17132"
- "9000221"
ms.date: ''
ms.openlocfilehash: 28cf302d750cd306202c31f28e0f195951a7f208
ms.sourcegitcommit: 29aa28c4fa26e71de062cb6319e48cd963fdf1fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/03/2022
ms.locfileid: "65862193"
---
# <a name="information-required-to-import-autopilot-device-hash"></a>Zum Importieren des Autopilot-Gerätehashs erforderliche Informationen

Möglicherweise versuchen Sie, den Gerätehash für ein Autopilot-Gerät zu importieren, das mit dem folgenden Fehler fehlschlägt:

"Einige Geräte wurden nicht importiert" und "808 - ZtdDeviceAssignedToOtherTenant". 

Sie müssen Microsoft-Support die folgenden Informationen zur Verfügung stellen, damit wir Sie bei der Behebung dieses Problems unterstützen können:

- **Geräte-CSV** Eine Kopie der CSV-Datei des Geräts, die den Fehler generiert hat.
- **Eigentumsnachweis** In der Regel handelt es sich dabei um eine Verkaufsrechnung oder eine Rechnung im PDF-Format.
    - Das Dokument muss in seiner ursprünglichen Form sein. Screenshots werden nicht akzeptiert.
    - Die Seriennummer, die Chassis-ID oder ein anderer eindeutiger Bezeichner muss im Dokument vorhanden sein. Für einige Anbieter müssen Sie möglicherweise zusätzliche Details zum gekauften Gerät anfordern, um diese Informationen zu finden.
    - Der Firmenname des Kunden muss im Dokument angezeigt werden.
    - Name des Händlers.

Wenn Sie nicht über den Hardwarehash des betroffenen Geräts verfügen, geben Sie auch die folgenden Daten an:

- **Diagnoseprotokolle** Melden Sie sich beim Gerät an, und führen Sie den Befehl `Mdmdiagnosticstool -area Autopilot -cab c:\out.cab`aus. Die `out.cab` Datei enthält wichtige Diagnosedaten, die bei der Problembehandlung helfen.

Stellen Sie sicher, dass Sie über die oben genannten Informationen verfügen, bevor Sie ein Supportticket öffnen.