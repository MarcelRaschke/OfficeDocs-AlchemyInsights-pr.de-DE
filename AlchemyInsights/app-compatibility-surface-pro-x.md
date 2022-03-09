---
title: App-Kompatibilität mit Microsoft Surface Pro X
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 5f4fda4fbb2b3ebef9c31026e75d9b0d28834f2c
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63308597"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>App-Kompatibilität mit Microsoft Surface Pro X

Anwendungen werden auf Geräten wie dem Surface Pro X unterschiedlich ausgeführt. Die meisten Apps sind kompatibel, es gibt jedoch einige Einschränkungen. Im Folgenden finden Sie eine Liste der Probleme, die beim Ausführen einer Anwendung auftreten könnten: 

**Treiber.** Treiber funktionieren, wenn sie für einen ARM-basierten Windows 10-PC konzipiert sind. Wenn ein Treiber nicht funktioniert, funktioniert auch die App – oder die Hardware, auf die sie sich stützt – nicht. Weitere Hilfe für Ihr Gerät finden Sie unter [Häufig gestellte Fragen zu ARM-basierten Windows 10-PCs](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5), oder wenden Sie sich diesbezüglich an den Hardwarehersteller.

**64-Bit-Apps (x64).** 64-Bit-Apps (x64) funktionieren nicht. Sie benötigen 64-Bit (ARM64)-Apps, 32-Bit (ARM32)-Apps oder 32-Bit (x86)-Apps. In der Regel gibt es von Apps auch 32-Bit-Versionen (x86), doch einige App-Entwickler bieten nur 64-Bit-Apps (x64).

**Angepasste Apps.** Bei Apps, die die Windows-Benutzerumgebung anpassen, wie Hilfstechnologien oder Cloudspeicher-Apps, können Probleme auftreten. Wenden Sie sich für weitere Informationen an den Hersteller der Anwendung.

**Antivirensoftware von Drittanbietern.** Einige Antivirensoftware von Drittanbietern kann nicht installiert werden. Windows Security hilft Ihnen, Ihre Daten während der unterstützten Lebensdauer Ihres Windows 10-Geräts zu schützen.

**Windows-Fax und -Scan.** Windows-Fax und -Scan ist auf einem Windows 10 ARM-basierten PC nicht verfügbar.

Wenn beim Installieren, Deinstallieren oder erneuten Installieren einer App Probleme auftreten, lesen Sie [Details zur Problembehandlung bei Apps](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details).

Außer in seltenen Fällen sollten alle Schlüsselwörter "ODER" statt "UND" sein.