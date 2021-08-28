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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112911"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive Anmeldefehler AADSTS50011

Wenn beim Anmelden bei der OneDrive-App die Fehlermeldung "AADSTS50011: Die in der Anforderung angegebene Antwort-URL stimmt nicht mit der Antwort überein" angezeigt wird, überprüfen Sie Folgendes:

Ihre OneDrive Version muss mindestens version 20.052.XXXX.XXXX entsprechen. Um Ihre Version zu überprüfen, klicken Sie auf das blaue OneDrive Symbol im Benachrichtigungsbereich, wählen Sie **Hilfe & Einstellungen > Einstellungen > Info** aus.

Ihr Netzwerk blockiert möglicherweise Datenverkehr zu **g.live.com** und **oneclient.sfx.ms.** Wenn dieser Datenverkehr blockiert ist, können OneDrive sich nicht selbst aktualisieren. Arbeiten Sie mit Ihrem Netzwerkadministrator, um sicherzustellen, dass Sie Zugriff auf diese URLs haben. [Diese Endpunkte](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) sollten für Kunden erreichbar sein, die Microsoft 365 Pläne verwenden.

Wenn Sie manuell eine aktuelle Version von OneDrive abrufen müssen, besuchen Sie [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
