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
ms.openlocfilehash: 1b96bd93b6cbe9bb59b03d6bc14cffd752f8a78e
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62754191"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive Anmeldefehler AADSTS50011

Wenn beim Anmelden bei der OneDrive App die Fehlermeldung "AADSTS50011: Die in der Anforderung angegebene Antwort-URL stimmt nicht mit der Antwort überein" angezeigt wird, überprüfen Sie Folgendes:

Ihre OneDrive Version muss mindestens der Version 20.052.XXXX.XXXX entsprechen. Um Ihre Version zu überprüfen, klicken Sie im Benachrichtigungsbereich auf das blaue OneDrive symbol, und wählen Sie **Hilfe & Einstellungen > Einstellungen > Info** aus.

Ihr Netzwerk blockiert möglicherweise den Datenverkehr zu **g.live.com** und **oneclient.sfx.ms**. Wenn dieser Datenverkehr blockiert wird, können OneDrive sich nicht selbst aktualisieren. Arbeiten Sie mit Ihrem Netzwerkadministrator, um sicherzustellen, dass Sie Zugriff auf diese URLs haben. [Diese Endpunkte](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges) sollten für Kunden erreichbar sein, die Microsoft 365 Pläne verwenden.

Wenn Sie eine aktuelle Version von OneDrive manuell abrufen müssen, besuchen Sie [https://aka.ms/getonedrive](https://aka.ms/getonedrive).
