---
title: Arbeiten mit iOS VPP-Anwendungsregel-ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083013"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeiten mit iOS-VPP-Anwendungen

Lesen [Sie, wie Sie iOS-Apps verwalten, die über ein Volumenkaufprogramm mit Microsoft Intune erworben wurden,](https://docs.microsoft.com/intune/vpp-apps-ios) um mehr über Features, Einschränkungen und Schritte zur Nutzung des Apple Volume Purchase-Programms und deren Unterstützung in Microsoft Intune zu erfahren.
  
 **Häufige Probleme:** "Ich habe meinen Benutzern eine iOS-VPP-App zugewiesen, aber die Installation ist fehlgeschlagen."
  
- Dies kann passieren, wenn ein einzelnes VPP-Token über mehrere Anbieter für die Verwaltung mobiler Geräte hinweg verwendet wird. VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden. Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in Intune hochladen.

- Die Installation kann auch fehlschlagen, wenn die Gesamtzahl der Installationen die Anzahl der Lizenzen überschreitet. Um einen Nutzungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur App-Lizenzenseite für **Intune Mobile-Apps.** \>  Informationen zum Freigeben verwendeter Lizenzen finden Sie in [diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
