---
title: OneDrive Anmeldefehler AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 5e3950988ddee6e45b5af44a2722e6f7303a069a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63183020"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive Anmeldefehler AADSTS50011

Wenn beim Anmelden bei der OneDrive-App die Fehlermeldung "AADSTS50011: Die in der Anforderung angegebene Antwort-URL stimmt nicht mit der Antwort überein" angezeigt wird, überprüfen Sie Folgendes:

Ihre OneDrive Version muss mindestens der Version 20.052.XXXX.XXXX entsprechen. Um Ihre Version zu überprüfen, klicken Sie im Benachrichtigungsbereich auf das blaue OneDrive Symbol, und wählen Sie **Hilfe & Einstellungen > Einstellungen > Info** aus.

Möglicherweise blockiert Ihr Netzwerk den Datenverkehr zu **g.live.com** und **oneclient.sfx.ms**. Wenn dieser Datenverkehr blockiert wird, können OneDrive sich nicht selbst aktualisieren. Arbeiten Sie mit Ihrem Netzwerkadministrator, um sicherzustellen, dass Sie Zugriff auf diese URLs haben. [Diese Endpunkte](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges) sollten für Kunden erreichbar sein, die Microsoft 365 Pläne verwenden.

Wenn Sie eine aktuelle Version von OneDrive manuell abrufen müssen, besuchen Sie [https://aka.ms/getonedrive](https://aka.ms/getonedrive).
