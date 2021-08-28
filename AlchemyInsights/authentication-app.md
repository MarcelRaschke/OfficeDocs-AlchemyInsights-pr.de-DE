---
title: Authentifizierungs-App
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082941"
---
# <a name="authentication-app"></a>Authentifizierungs-App

Wenn Sie ein globaler Administrator sind, können Sie mithilfe der [Anmeldediagnose](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzeranmeldung diagnostizieren.

1. Starten Sie die Diagnose, indem Sie auf die Schaltfläche["Diagnose starten"](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)klicken. 
1. Suchen Sie das zu analysierende Ereignis, indem Sie die Details zu Benutzer, Anwendung, Zeitpunkt der Anmeldung, Anforderungs-ID oder Korrelations-ID eingeben.
1. Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.

**Überprüfen Sie das zutreffende Szenario:**

1. Wenn ein Benutzer keine Pushbenachrichtigung in der Microsoft Authenticator-App erhält, überprüfen Sie, ob er nicht unter den blockierten MFA-Benutzern angezeigt wird, wie unter ["Blockieren und Aufheben](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)der Blockierung von Benutzern" beschrieben.
1. Wenn der Benutzer nicht für MFA blockiert ist, aber keine Pushbenachrichtigung erhält, kann er die Microsoft Authenticator-App öffnen, die die ausstehenden Genehmigungsanforderungen abruft.
1. Als alternative Anmeldemethode kann der Benutzer auch auf eine andere Weise auf "Anmelden" klicken und einen Überprüfungscode aus meiner mobilen App verwenden.
1. Die Microsoft Authenticator-App ist die einzige verfügbare Methode für viele Benutzer. [Erfahren Sie mehr über Sicherheitsstandards,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)überprüfen Sie Authenticator Häufig gestellte Fragen zur [App,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) und erfahren Sie, wie Sie diese beheben können.
 
**Empfohlene Videos**

[So richten Sie Authenticator App auf einem neuen Telefon (2 Minuten) ein.](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
