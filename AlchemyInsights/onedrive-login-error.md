---
title: OneDrive Anmeldefehler AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 7983459b302e2d619dee5e15a822afe9b3fd0056
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61989738"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive Anmeldefehler AADSTS50011

Wenn beim Anmelden bei der OneDrive App die Fehlermeldung "AADSTS50011: Die in der Anforderung angegebene Antwort-URL stimmt nicht mit der Antwort überein" angezeigt wird, überprüfen Sie Folgendes:

Ihre OneDrive Version muss mindestens der Version 20.052.XXXX.XXXX entsprechen. Um Ihre Version zu überprüfen, klicken Sie auf das blaue OneDrive Symbol im Benachrichtigungsbereich, wählen Sie **Hilfe & Einstellungen > Einstellungen > Info** aus.

Möglicherweise blockiert Ihr Netzwerk Datenverkehr zu **g.live.com** und **oneclient.sfx.ms.** Wenn dieser Datenverkehr blockiert wird, können OneDrive sich nicht selbst aktualisieren. Arbeiten Sie mit Ihrem Netzwerkadministrator, um sicherzustellen, dass Sie Zugriff auf diese URLs haben. [Diese Endpunkte](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges) sollten für Kunden erreichbar sein, die Microsoft 365 Pläne verwenden.

Wenn Sie eine aktuelle Version von OneDrive manuell abrufen müssen, besuchen Sie [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
