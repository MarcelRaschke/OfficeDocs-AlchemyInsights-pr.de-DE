---
title: Konfigurieren von Endpunkt-DLP
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3200001"
- "6108"
ms.date: 05/26/2022
ms.openlocfilehash: 045d7234b783da256d2f83114bf096b86b8a540c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66412717"
---
# <a name="configure-endpoint-dlp"></a>Konfigurieren von Endpunkt-DLP

Verhinderung von Datenverlust am Endpunkt (Endpunkt-DLP) erweitert die Aktivitätsüberwachung und die Schutzfunktionen von DLP auf vertrauliche Elemente, die physisch auf Windows 10-, Windows 11- und macOS-Geräten (Catalina 10.15 und höher) gespeichert sind. Nachdem Geräte in den Microsoft Purview-Lösungen eingebunden wurden, werden die Informationen zu den Aktionen, die Benutzer mit den vertraulichen Elementen ausführen, im Aktivitäten-Explorer angezeigt, und Sie können Schutzmaßnahmen für diese Elemente mithilfe von DLP-Richtlinien erzwingen.

So führen Sie die ersten Schritte mit Endpunkt-DLP aus

- Stellen Sie sicher, dass Sie über die geeignete SKU/Abonnementlizenzierung verfügen. Weitere Informationen finden Sie unter [SKU/Abonnement-Lizenzierung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Überprüfen Sie die Berechtigungen, die erforderlich sind, um die Geräteverwaltung zu aktivieren, auf die Onboardingseite zuzugreifen oder die Geräteüberwachung ein- und auszuschalten. Weitere Informationen finden Sie unter [Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Führen Sie ein Onboarding der Geräte in die Geräteverwaltung aus, indem Sie dem Verfahren für das Onboarding von Geräten folgen. Weitere Informationen finden Sie unter [Onboarding von Geräten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Erstellen Sie DLP-Richtlinien zum Schutz Ihrer vertraulichen Elemente. Informationen hierzu finden Sie unter [Szenarien für Endpunkt-DLP-Richtlinien](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using#endpoint-dlp-policy-scenarios).

Weitere Informationen zur Verhinderung von Datenverlust am Endpunkt finden Sie unter [Informationen zu Endpunkt-DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Wichtige Datenerfassungsschritte, falls Support benötigt wird:**

1. [MDATP Client Analyzer-Vorschauversion](https://aka.ms/betamdatpanalyzer) herunterladen.
1. Führen Sie das Tool über das CMD-Fenster als Administrator aus:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd -t**

1. Wenn Sie mit **Geben Sie die Anzahl der Minuten ein, in denen die Ablaufverfolgungen erfasst werden soll** aufgefordert werden, geben Sie Dauer, die für die Ausführung des Szenarios erforderlich ist, in Minuten ein.
1. Führen Sie das Szenario aus.

Erfassen Sie die ZIP-Dateiausgabe, um sie dem Supportmitarbeiter zu übergeben.
