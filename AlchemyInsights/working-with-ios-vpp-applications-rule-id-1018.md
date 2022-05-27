---
title: Arbeiten mit iOS VPP-Anwendungsregel-ID 1018
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: cbc2518d7cbaa6fde97c095d57f97c0083d60586
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65729656"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeiten mit iOS VPP-Anwendungen

Lesen Sie[, wie Sie iOS Apps verwalten, die über ein Volumenkaufprogramm erworben wurden, mit Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios), um mehr über Features, Einschränkungen und Schritte zu erfahren, um das Apple Volume Purchase Program und den Support dafür in Microsoft Intune zu nutzen.
  
 **Häufige Probleme:** "Ich habe meinen Benutzern eine iOS VPP-App zugewiesen, aber die Installation ist fehlgeschlagen."
  
- Dies kann passieren, wenn ein einzelnes VPP-Token über mehrere Anbieter für die Verwaltung mobiler Geräte hinweg verwendet wird. VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden. Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in Intune hochladen.

- Die Installation kann auch fehlschlagen, wenn die Gesamtanzahl der Installationen die Anzahl der Lizenzen überschreitet. Um einen Nutzungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur Seite Intune **App-Lizenzen** für **mobile Apps**\>. Informationen zum Freigeben von Lizenzen in Verwendung finden Sie [in diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
