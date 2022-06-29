---
title: Authentifizierungs-App
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003252"
- "9909"
ms.date: 03/24/2021
ms.openlocfilehash: 2cd7208bfdb6ca382f17bcb868126761c2ca724d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66260938"
---
# <a name="authentication-app"></a>Authentifizierungs-App

Wenn Sie ein globaler Admin sind, können Sie mithilfe der [Anmeldediagnose](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzeranmeldung diagnostizieren.

1. Starten Sie die Diagnose, indem Sie auf die Schaltfläche "[Diagnose starten](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" klicken. 
1. Suchen Sie das zu analysierende Ereignis, indem Sie die Details eingeben, die Sie über den Benutzer, die Anwendung, den Zeitpunkt der Anmeldung, die Anforderungs-ID oder die Korrelations-ID haben.
1. Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.

**Überprüfen Sie das anwendbare Szenario:**

1. Wenn ein Benutzer keine Pushbenachrichtigung in der Microsoft Authenticator-App erhält, vergewissern Sie sich, dass er nicht unter den MFA-blockierten Benutzern angezeigt wird, wie unter ["Blockieren und Aufheben der Blockierung von Benutzern](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" beschrieben.
1. Wenn der Benutzer nicht für MFA blockiert ist, aber keine Pushbenachrichtigung empfängt, kann er die Microsoft Authenticator-App öffnen, wodurch die ausstehenden Genehmigungsanforderungen abgerufen werden.
1. Als alternative Anmeldemethode kann der Benutzer auch auf eine andere Weise auf "Anmelden" klicken und einen Überprüfungscode aus meiner mobilen App auswählen.
1. Die Microsoft Authenticator-App ist die einzige verfügbare Methode für viele Benutzer. [Erfahren Sie mehr über Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), überprüfen Sie die häufig gestellten Fragen zur [Authenticator-App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) , um häufig gestellte Fragen zu erhalten und wie Sie diese beheben können.
 
**Empfohlene Videos**

[Einrichten der Authenticator-App auf einem neuen Telefon (2 Minuten)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
