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
ms.openlocfilehash: 91af1b450bc395c32030366c51b53ade95a95012
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62658318"
---
# <a name="authentication-app"></a>Authentifizierungs-App

Wenn Sie ein globaler Administrator sind, können Sie schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzeranmeldung mithilfe der [Anmeldediagnose](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) diagnostizieren.

1. Starten Sie die Diagnose, indem Sie auf die Schaltfläche "[Diagnose starten](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" klicken. 
1. Suchen Sie das zu analysierende Ereignis, indem Sie die Details eingeben, die Sie über den Benutzer, die Anwendung, den Zeitpunkt der Anmeldung, die Anforderungs-ID oder die Korrelations-ID haben.
1. Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.

**Überprüfen Sie das zutreffende Szenario:**

1. Wenn ein Benutzer keine Pushbenachrichtigung in der Microsoft Authenticator App erhält, stellen Sie sicher, dass er nicht unter den blockierten MFA-Benutzern angezeigt wird, wie unter ["Blockieren und Aufheben der Blockierung von Benutzern](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" beschrieben.
1. Wenn der Benutzer nicht für MFA blockiert ist, aber keine Pushbenachrichtigung erhält, kann er die Microsoft Authenticator-App öffnen, die die ausstehenden Genehmigungsanforderungen abruft.
1. Als alternative Anmeldemethode kann der Benutzer auch auf eine andere Weise auf "Anmelden" klicken und einen Überprüfungscode aus meiner mobilen App verwenden.
1. Die Microsoft Authenticator-App ist die einzige verfügbare Methode für viele Benutzer. [Weitere Informationen zu Sicherheitsstandards finden Sie](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [in den häufig gestellten Fragen Authenticator App](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) und wie Sie diese beheben können.
 
**Empfohlene Videos**

[So richten Sie Authenticator App auf einem neuen Telefon (2 Minuten) ein](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
