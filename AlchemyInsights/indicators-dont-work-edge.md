---
title: Indikatoren funktionieren nicht im Edge-Browser
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9005470"
- "11230"
ms.date: 05/25/2021
ms.openlocfilehash: 52ebe787f3f5fdf5d7e1589949ba9e8b8e2b923d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66296200"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatoren funktionieren nicht im Edge-Browser

Nachdem Sie einen Indikator erstellt haben, wird er von Edge (Smartscreen) nicht mehr unterstützt. Weitere Informationen finden Sie unter [Erstellen von Indikatoren für IPs und URLs/Domänen](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Schritt 1: Stellen Sie Folgendes sicher

- Überprüfen Sie, ob der Indikator richtig ist (keine Tippfehler in IP/URL, richtige Aktion, die richtigen RBAC-Gruppen).
- Warten Sie die Mindestdauer von 2 Stunden nach dem Erstellen des Indikators ab, um mögliche Wartezeiten zu berücksichtigen.
- Vergewissern Sie sich, dass das System/die Systeme in Microsoft Defender für Endpunkt integriert sind.
- Stellen Sie sicher, dass das System/die Systeme mit der Cloud kommunizieren können.
- Stellen Sie sicher, dass Smartscreen aktiviert und erreichbar ist, indem Sie zur [Testwebsite](https://demo.smartscreen.msft.net) wechseln.

## <a name="step-2-troubleshoot-the-potential-issue"></a>Schritt 2: Beheben Sie das potenzielle Problem

- Stellen Sie sicher, dass der Kunde die Anforderungen erfüllt. Weitere Details finden Sie unter [Erstellen von Indikatoren für IPs und URLs/Domänen](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Stellen Sie sicher, dass Sie die neueste Version des Edge-Browsers ausführen. Informationen zur neuesten Version finden Sie unter [Finden Sie heraus, über welche Version von Microsoft Edge Sie verfügen](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Starten Sie den Edge-Browser neu.
- Navigieren Sie zur Website, für die Sie einen Indikator eingerichtet haben. Wenn die Website nicht wie erwartet angezeigt wird, fahren Sie mit Schritt 3 fort. 

## <a name="step-3-collect-data"></a>Schritt 3: Sammeln Sie Daten

- Sammeln sie **MDEClientAnalyzer** Diagnosedaten. Anweisungen finden Sie unter [Client Analyzer auf Windows ausführen](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/run-analyzer-windows).
- Wenn Sie mit dem Installieren und Sammeln einer Fiddler-Ablaufverfolgung vertraut sind, lesen Sie [Telerik Fiddler](http://www.telerik.com/fiddler).
- Wenn Sie die Anleitung vom Microsoft-Support bevorzugen, wählen Sie das Supportsymbol unten aus, um einen Support-Fall zu öffnen.
