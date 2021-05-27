---
title: Indikatoren funktionieren nicht im Edge-Browser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651491"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatoren funktionieren nicht im Edge-Browser

Nachdem Sie einen Indikator erstellt haben, wird er von Edge (Smartscreen) nicht mehr unterstützt. Weitere Informationen finden Sie unter [Erstellen von Indikatoren für IPs und URLs/Domänen](/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Schritt 1: Stellen Sie Folgendes sicher

- Überprüfen Sie, ob der Indikator richtig ist (keine Tippfehler in IP/URL, richtige Aktion, die richtigen RBAC-Gruppen).
- Warten Sie die Mindestdauer von 2 Stunden nach dem Erstellen des Indikators ab, um mögliche Wartezeiten zu berücksichtigen.
- Vergewissern Sie sich, dass das System/die Systeme in Microsoft Defender für Endpunkt integriert sind.
- Stellen Sie sicher, dass das System/die Systeme mit der Cloud kommunizieren können.
- Stellen Sie sicher, dass Smartscreen aktiviert und erreichbar ist, indem Sie zur [Testwebsite](https://demo.smartscreen.msft.net) wechseln.

## <a name="step-2-troubleshoot-the-potential-issue"></a>Schritt 2: Beheben Sie das potenzielle Problem

- Stellen Sie sicher, dass der Kunde die Anforderungen erfüllt. Weitere Details finden Sie unter [Erstellen von Indikatoren für IPs und URLs/Domänen](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Stellen Sie sicher, dass Sie die neueste Version des Edge-Browsers ausführen. Informationen zur neuesten Version finden Sie unter [Finden Sie heraus, über welche Version von Microsoft Edge Sie verfügen](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Starten Sie den Edge-Browser neu.
- Navigieren Sie zur Website, für die Sie einen Indikator eingerichtet haben. Wenn die Website nicht wie erwartet angezeigt wird, fahren Sie mit Schritt 3 fort. 

## <a name="step-3-collect-data"></a>Schritt 3: Sammeln Sie Daten

- Sammeln Sie **MDEClientAnalyzer** Diagnosedaten. Anweisungen finden Sie unter [Probleme beim Onboarding von Microsoft Defender für Endpunkt auf Computern](issues-with-onboarding-machines.md).
- Wenn Sie mit dem Installieren und Sammeln einer Fiddler-Ablaufverfolgung vertraut sind, lesen Sie [Telerik Fiddler](http://www.telerik.com/fiddler).
- Wenn Sie die Anleitung vom Microsoft-Support bevorzugen, wählen Sie das Supportsymbol unten aus, um einen Support-Fall zu öffnen.
