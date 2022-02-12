---
title: Intune-Gerätebestand
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: b2a92ebdc5d70f4db5487264a8245275b528f7ab
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62604407"
---
# <a name="intune-device-inventory"></a>Intune-Gerätebestand

Das Blatt "Geräte" bietet dem Administrator einen Einblick in die in Intune verwalteten Geräte auf Gerätebasis. Die angezeigten Informationen umfassen: Hardware, entdeckte Anwendungen, Gerätecompliancestatus und Gerätekonfigurationsstatus.

Bestandsdaten für Hardware und entdeckte Anwendungen werden in einem siebentägigen Zyklus gesammelt. Die gemeldeten Anwendungen und spezifischen Elemente der Hardware unterscheiden sich je nach Betriebssystem des Geräts und je nachdem, ob das Gerät in Privat- oder Firmenbesitz ist.

Weitere Informationen finden Sie unter [Anzeigen von Gerätedetails in Intune](https://docs.microsoft.com/intune/device-inventory).

**Häufig gestellte Fragen**

F: Ich erhalte keine vollständige Bestandsliste der Anwendungen auf bei Intune registrierten Windows-Geräten. Warum nicht?

A: Gegenwärtig werden nur moderne Apps für als Unternehmensgeräte identifizierte Windows 10-PCs aufgeführt. Intune sammelt keine Informationen über Win32-Anwendungen, die auf diesen Geräten installiert sind.

F: Warum werden Telefonnummern nicht von allen Geräten gesammelt?

A: Telefone, die in Intune als Unternehmensgeräte kategorisiert sind, werden nicht mit ihrer vollständigen Telefonnummer identifiziert, wenn Sie z. B. einen Bestandsbericht für mobile Geräte ausführen. Bring-Your-Own-Device-Telefonnummern werden immer teilweise mit Sternchen (****) maskiert und zeigen nur die letzten vier Ziffern.