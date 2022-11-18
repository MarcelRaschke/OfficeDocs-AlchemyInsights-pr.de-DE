---
title: OneDrive-Anmeldefehler AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: d747f1589aa108b351702b9f40db4bf9b4e325dc
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66387021"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive-Anmeldefehler AADSTS50011

Wenn beim Anmelden bei der OneDrive-App die Fehlermeldung "AADSTS50011: Die in der Anforderung angegebene Antwort-URL stimmt nicht mit der Antwort überein" angezeigt wird, überprüfen Sie Folgendes:

Ihre OneDrive-Version muss der Version 20.052.XXXX.XXXX entsprechen oder größer sein. Um Ihre Version zu überprüfen, klicken Sie im Infobereich auf das blaue OneDrive-Symbol, und wählen Sie **"Hilfe & Einstellungen > Einstellungen > Info**" aus.

Ihr Netzwerk blockiert möglicherweise den Datenverkehr zu **g.live.com** und **oneclient.sfx.ms**. Wenn dieser Datenverkehr blockiert wird, kann OneDrive sich nicht selbst aktualisieren. Arbeiten Sie mit Ihrem Netzwerkadministrator zusammen, um sicherzustellen, dass Sie Zugriff auf diese URLs haben. [Diese Endpunkte](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges) sollten für Kunden erreichbar sein, die Microsoft 365-Pläne verwenden.

Wenn Sie manuell eine aktuelle Version von OneDrive abrufen müssen, besuchen Sie [https://aka.ms/getonedrive](https://aka.ms/getonedrive).
