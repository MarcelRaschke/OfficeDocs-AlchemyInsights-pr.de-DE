---
title: Probleme beim Anmelden bei Anwendungen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004355"
- "7788"
ms.date: 01/16/2021
ms.openlocfilehash: f694ad3fbf1fcdd61c201e8198f81b221bf603ac
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66287597"
---
# <a name="issues-signing-in-to-applications"></a>Probleme beim Anmelden bei Anwendungen

Führen Sie die folgenden Schritte durch, um die Ursache zu ermitteln oder Probleme im Zusammenhang mit der Benutzeranmeldung zu diagnostizieren:

1. Starten Sie die [Anmeldediagnose](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Suchen Sie das zu analysierende Ereignis, indem Sie die Details über den Benutzer, die Anwendung, den Zeitpunkt der Anmeldung, die Anfrage-ID oder die Korrelations-ID eingeben.
3. Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.

Im Folgenden sind einige häufige Probleme aufgeführt, die bei der Anmeldung bei Anwendungen auftreten können:

1. Sie oder der Benutzer **haben eine Azure AD-Anmeldung abgeschlossen, sehen aber eine unerwartete Eingabeaufforderung** – Siehe die Artikel [Unerwartete Zustimmungsaufforderung beim Anmelden bei einer Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) und [Unerwarteter Fehler bei der Durchführung der Zustimmung zu einer Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Sie oder ein Benutzer **haben sich direkt bei einer Anwendung angemeldet, können sich aber nicht über einen Deeplink im benutzerdefinierten Portal oder im Zugriffsbereich anmelden**: Siehe [Probleme beim Anmelden bei einer Anwendung über Azure AD Meine Apps beheben](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Sie oder ein Benutzer **haben eine Azure AD-Anmeldung abgeschlossen, aber die Anwendung zeigt eine Fehlermeldung an und lässt den Benutzer den Anmeldevorgang nicht abschließen**: Das Problem ist, dass die App die von Azure AD ausgegebene Antwort nicht akzeptiert hat. Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) zur Problembehandlung durch.
4. Sie oder ein Benutzer können sich **nicht bei einer Nicht-Galerie-Anwendung anmelden, die für das Single Sign-On mit Kennwort konfiguriert ist**: Befolgen Sie die Anleitung in [diesen Schritten](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) zur Problembehandlung.
5. Sie oder ein Benutzer können sich **nicht bei einer Azure AD-Galerie-Anwendung anmelden, die für Single Sign-On mit Kennwort konfiguriert ist**: Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) zur Problembehebung durch.
6. Sie oder ein Benutzer **können sich nicht bei einer Microsoft-Anwendung anmelden**: Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) zur Problembehandlung durch.
7. Sie oder ein Benutzer **können sich nicht bei einer Nicht-Galerie-Anwendung anmelden, die für Verbund-Single-Sign-on konfiguriert ist**: Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) zur Problembehandlung durch.
8. Sie oder ein Benutzer **können sich nicht bei einer Azure AD-Galerie-Anwendung anmelden, die für Verbund-Single Sign-On konfiguriert ist**: Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) zur Problembehebung durch.
9. Sie oder ein Benutzer **können sich nicht bei einer selbstentwickelten Anwendung anmelden**: Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) zur Problembehandlung durch.
10. Sie oder ein Benutzer **können sich über den Azure AD-Anwendungsproxy nicht bei einer lokalen Anwendung anmelden**: Führen Sie [diese Schritte](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) zur Problembehandlung durch.

