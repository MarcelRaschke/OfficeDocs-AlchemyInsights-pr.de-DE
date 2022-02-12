---
title: Konfigurieren von Endpunkt-DLP
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 6d13d03bb76efa7ca6c2c42eace5c3669688be01
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62593210"
---
# <a name="configure-endpoint-dlp"></a>Konfigurieren von Endpunkt-DLP

Microsoft Endpunkt-DLP bietet Ihnen die Möglichkeit, Schutz- und Überwachungsfunktionen von DLP auf vertrauliche Informationen auf Windows 10-Geräten zu erweitern. Nachdem die Geräte in die Geräteverwaltung integriert wurden, können Sie DLP-Richtlinien erstellen, um Schutzmaßnahmen für Objekte durchzusetzen. Der Aktivitäten-Explorer kann verwendet werden, um die Aktivität für vertrauliche Elemente zu überwachen. Weitere Informationen finden Sie unter [Onboarding von Geräten für die Geräteverwaltung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

So führen Sie die ersten Schritte mit Endpunkt-DLP aus

- Stellen Sie sicher, dass Sie über die geeignete SKU/Abonnementlizenzierung verfügen. Weitere Informationen finden Sie unter [SKU/Abonnement-Lizenzierung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Überprüfen Sie die erforderlichen Berechtigungen, um die Geräteverwaltung zu aktivieren, auf die Onboardingseite zuzugreifen oder die Geräteüberwachung zu aktivieren/zu deaktivieren. Weitere Informationen finden Sie unter [Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Führen Sie ein Onboarding der Geräte in die Geräteverwaltung aus, indem Sie dem Verfahren für das Onboarding von Geräten folgen. Weitere Informationen finden Sie unter [Onboarding von Geräten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Erstellen Sie DLP-Richtlinien zum Schutz Ihrer vertraulichen Elemente. Informationen hierzu finden Sie unter [Szenarien für Endpunkt-DLP-Richtlinien](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using#endpoint-dlp-policy-scenarios).

Weitere Informationen zu Microsoft Endpunkt-DLP finden Sie unter [Informationen zu Microsoft 365 Endpunkt-DLP (Data Loss Prevention, Verhinderung von Datenverlust) (Vorschau)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Wichtige Datenerfassungsschritte, falls Support benötigt wird:**

1. [MDATP Client Analyzer-Vorschauversion](https://aka.ms/betamdatpanalyzer) herunterladen.
1. Führen Sie das Tool über das CMD-Fenster als Administrator aus:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Wenn Sie mit **Geben Sie die Anzahl der Minuten ein, in denen die Ablaufverfolgungen erfasst werden soll** aufgefordert werden, geben Sie Dauer, die für die Ausführung des Szenarios erforderlich ist, in Minuten ein.
1. Führen Sie das Szenario aus.

Erfassen Sie die ZIP-Dateiausgabe, um sie dem Supportmitarbeiter zu übergeben.
