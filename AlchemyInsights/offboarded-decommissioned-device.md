---
title: Probleme beim Entfernen eines offboardierten oder außer Betrieb genommenen Geräts aus dem Gerätebestand
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324443"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Probleme beim Entfernen eines offboardierten oder außer Betrieb genommenen Geräts aus dem Gerätebestand

Microsoft Defender für Endpunkt lässt derzeit nicht zu, den Gerätedatensatz eines offboardierten oder außer Betrieb genommenen Geräts manuell aus dem Gerätebestand zu entfernen.

Aus Sicherheitsgründen bleibt das Gerät bis zu 180 Tage lang als Verlaufsdatensatz im Portal. Die Gerätedaten werden jedoch gemäß ihrem konfigurierten Aufbewahrungszeitraum gelöscht.

**Hinweis:** Ein offboardiertes oder außer Betrieb genommenes Gerät wechselt nach sieben Tagen automatisch in den **inaktiven** Zustand. Darüber hinaus werden Geräte, die in den letzten 30 Tagen nicht aktiv waren, nicht in die Daten einbezogen, die Ihre Organisation Bedrohungs- und Sicherheitsrisikomanagement Belichtungsbewertung oder Microsoft-Sicherheitsbewertung für Geräte widerspiegeln.
 
Wenn Bestimmte Geräte in der Geräteinventuransicht weiterhin nicht angezeigt werden sollen, versuchen Sie, ein Gerätetag zu platzieren, um das außer Betrieb genommene Gerät aus der Gerätebestandsansicht herauszufiltern.

Weitere Informationen finden Sie unter:

[Offboarding von Geräten aus dem Microsoft Defender für Endpunkt-Dienst](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Belichtungsbewertung in Bedrohungs- und Sicherheitsrisikomanagement](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Beheben fehlerhafter Sensoren in Microsoft Defender für Endpunkt](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Effektive Verwendung von Tagging (Teil 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Effektive Verwendung von Tagging (Teil 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Effektive Verwendung von Tagging (Teil 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




