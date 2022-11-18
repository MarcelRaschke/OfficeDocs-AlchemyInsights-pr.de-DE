---
title: Probleme mit bedingtem Zugriff
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004349"
- "7768"
ms.date: 01/25/2021
ms.openlocfilehash: 2c6419df04caa68838690018e6a165bd08c90806
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66393159"
---
# <a name="conditional-access-issues"></a>Probleme mit bedingtem Zugriff

**Beheben von Problemen mit der Anmeldediagnose**

Mithilfe der [Anmeldediagnose](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) können Sie schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzeranmeldung diagnostizieren:

1. Starten Sie die Anmeldediagnose.
1. Suchen Sie das zu analysierende Ereignis, indem Sie die Details eingeben, die Sie über den Benutzer, die Anwendung, den Zeitpunkt der Anmeldung, die Anforderungs-ID oder die Korrelations-ID haben.
1. Überprüfen Sie die Diagnoseergebnisse mit den Details zu den Ereignissen und den Aktionen, die Sie ausführen können, um Änderungen vorzunehmen (falls Änderungen erforderlich sind).

**Schritte zur Problembehandlung bei einer Anmeldung** 

1. Navigieren Sie zur Azure AD-Anmeldeseite.
1. Filtern Sie Anmeldungen nach Benutzer, Zeitraum, Anwendung, Status, Client-App usw.
1. Wählen Sie ein Anmeldeereignis aus, und zeigen Sie die Registerkarte für bedingten Zugriff an, um zu sehen, welche Richtlinien ausgewertet wurden.
1. Klicken Sie auf die Zeile einer Richtlinie, um die Richtliniendetails anzuzeigen und zu verstehen, warum sie angewendet wurde.

**Tools zur Problembehandlung für eine Richtlinie für bedingten Zugriff**

- Im Berichtsmodus können Sie eine Richtlinie auswerten, ohne die Benutzer zu beeinträchtigen.
- Mit dem Was-wäre-wenn-Tool können Sie Anmeldeereignisse simulieren und sehen, welche Richtlinien gelten.
- Einblicke und Berichtsarbeitsmappen zeigen die Auswirkungen jeder Richtlinie in Echtzeit an.

**Grundlegende Schutzrichtlinien**

Baseline Protection-Richtlinien sind veraltet. Sie werden nicht mehr erzwungen und bald aus Azure-Portal entfernt. Es wird empfohlen, [Sicherheitsstandards zu](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) aktivieren.

Weitere Informationen zum bedingten Zugriff finden Sie unter:

[Bewährte Methoden für bedingten Zugriff in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
 [Bedingungen im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
 [Steuerelemente im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
 [Speicherorte im bedingten Zugriff ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
