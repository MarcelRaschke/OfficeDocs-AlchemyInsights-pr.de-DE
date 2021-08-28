---
title: Probleme mit bedingtem Zugriff
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069963"
---
# <a name="conditional-access-issues"></a>Probleme mit bedingtem Zugriff

**Beheben von Problemen mit der Anmeldediagnose**

Mithilfe der [Anmeldediagnose](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)können Sie schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzeranmeldung diagnostizieren:

1. Starten Sie die Anmeldediagnose.
1. Suchen Sie das zu analysierende Ereignis, indem Sie die Details zu Benutzer, Anwendung, Zeitpunkt der Anmeldung, Anforderungs-ID oder Korrelations-ID eingeben.
1. Überprüfen Sie die Diagnoseergebnisse mit den Details der Ereignisse und der Aktionen, die Sie ausführen können, um Änderungen vorzunehmen (falls Änderungen erforderlich sind).

**Schritte zur Problembehandlung bei einer Anmeldung** 

1. Navigieren Sie zur Azure AD-Anmeldeseite.
1. Filtern von Anmeldungen nach Benutzer, Zeitraum, Anwendung, Status, Client-App usw.
1. Wählen Sie ein Anmeldeereignis aus, und zeigen Sie die Registerkarte "Bedingter Zugriff" an, um anzuzeigen, welche Richtlinien ausgewertet wurden.
1. Klicken Sie auf die Zeile einer Richtlinie, um die Richtliniendetails anzuzeigen und zu verstehen, warum sie angewendet wurde.

**Tools zur Problembehandlung einer Richtlinie für bedingten Zugriff**

- Im Modus "Nur Bericht" können Sie eine Richtlinie auswerten, ohne die Benutzer zu beeinträchtigen.
- Mit dem Was-wäre-wenn-Tool können Sie Anmeldeereignisse simulieren und sehen, welche Richtlinien gelten.
- Insights und Berichtsarbeitsmappe zeigt die Auswirkungen jeder Richtlinie in Echtzeit an.

**Grundlegende Schutzrichtlinien**

Baseline Protection-Richtlinien sind veraltet. Sie werden nicht mehr erzwungen und bald aus dem Azure-Portal entfernt. Es wird empfohlen, [die Sicherheitsstandards zu](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)aktivieren.

Weitere Informationen zum bedingten Zugriff finden Sie unter:

[Bewährte Methoden für bedingten Zugriff in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Bedingungen im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Steuerelemente im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Speicherorte im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
