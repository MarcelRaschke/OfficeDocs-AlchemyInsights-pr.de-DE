---
title: Arbeiten mit iOS-VPP-Anwendungen – Regel-ID 1018
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "6700004"
- "1018"
ms.date: 04/21/2020
ms.openlocfilehash: da3b8088fc68284fa43d93a230e45e5a14dec7b7
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66524884"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeiten mit iOS-VPP-Anwendungen

Lesen Sie[, wie Sie iOS-Apps verwalten, die über ein Volumenkaufprogramm erworben wurden, mit Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios), um mehr über Features, Einschränkungen und Schritte zu erfahren, um das Apple Volume Purchase Program und den Support dafür in Microsoft Intune zu nutzen.
  
 **Häufige Probleme:** "Ich habe meinen Benutzern eine iOS-VPP-App zugewiesen, aber die Installation ist fehlgeschlagen."
  
- Dies kann passieren, wenn ein einzelnes VPP-Token über mehrere Anbieter für die Verwaltung mobiler Geräte hinweg verwendet wird. VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden. Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in Intune hochladen.

- Die Installation kann auch fehlschlagen, wenn die Gesamtanzahl der Installationen die Anzahl der Lizenzen überschreitet. Um einen Nutzungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur Seite Intune **App-Lizenzen** für **mobile Apps**\>. Informationen zum Freigeben von Lizenzen in Verwendung finden Sie [in diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
