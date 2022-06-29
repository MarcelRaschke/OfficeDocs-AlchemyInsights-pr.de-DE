---
title: Problembehandlung bei SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.topic: article
audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003259"
- "6128"
ms.date: 03/04/2021
ms.openlocfilehash: 441494b4fce91c659c99ce39f939e02e492af915
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66251326"
---
# <a name="troubleshoot-sspr"></a>Problembehandlung bei SSPR

**Ich habe Probleme beim Konfigurieren der Kennwortzurücksetzung**

- Wenn Sie Administrator sind und wissen möchten, wie Sie die Self-Service-Kennwortzurücksetzung aktivieren, lesen Sie [das Lernprogramm zum Aktivieren von SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), um die Kennwortzurücksetzung für Ihre Organisation zu konfigurieren. Möglicherweise möchten Sie auch die [Lizenzierungsanforderungen](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) überprüfen. Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
    - **Nur Cloudbenutzer** – alle Office 365 (O365) kostenpflichtige SKU oder Azure AD Basic
    - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
- Weitere Fragen zur Self-Service-Kennwortzurücksetzung finden Sie in [unseren häufig gestellten Fragen](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ich erhalte eine Fehlermeldung**

Lesen Sie diesen Artikel, um häufige Fehler und deren Lösungen zu finden: [Behandeln von Problemen mit der Self-Service-Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich habe ein Problem mit meiner Kennwortzurücksetzungsrichtlinie**

- Wenn Sich Ihre Kennwortzurücksetzungsrichtlinie nicht wie erwartet verhält oder Sie Fragen zu Kennwortzurücksetzungsrichtlinien haben, lesen Sie diesen Artikel: [Kennwortrichtlinien und Einschränkungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Richtlinien für die Kennwortzurücksetzung gelten nicht für Administratoren. Microsoft erzwingt eine starke Zwei-Gate-Kennwortzurücksetzungsrichtlinie für jede Azure-Administratorrolle. Stellen Sie sicher, dass Sie tests mit einem Benutzer, der kein Administrator ist. Weitere Informationen zur Administratorrücksetzungsrichtlinie finden Sie in diesem Artikel: Unterschiede bei der [Administratorrücksetzungsrichtlinie.For](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences) more information on the administrator reset policy, see this article: Administrator reset policy differences.

**Ich möchte nicht, dass meine Benutzer zusätzliche Sicherheitsinformationen für die Kennwortzurücksetzung registrieren.**

Sie können Daten (E-Mail- und Telefonattribute) für Ihre Benutzer mithilfe einer API, PowerShell oder Azure AD Connect vorab auffüllen. So erfahren Sie, wie Sie lesen:

- [Bereitstellen der Kennwortzurücksetzung, ohne dass Benutzer sich registrieren müssen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Welche Daten werden von der Kennwortzurücksetzung verwendet?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich möchte, dass meine Benutzer ihre zusätzlichen Sicherheitsinformationen für die Kennwortzurücksetzung registrieren.**

1. Lassen Sie Ihre Benutzer ihre Sicherheitsinformationen für die Self-Service-Kennwortzurücksetzung registrieren, indem Sie sie an [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info) weiterleiten.
1. Nachdem Daten für den Benutzer (vom Benutzer oder vom Administrator) aufgefüllt wurden, leiten Sie Den Benutzer zu [aka.ms/sspr](https://passwordreset.microsoftonline.com/) , damit Ihre Benutzer ihre eigenen Kennwörter zurücksetzen können.
1. Wenn Benutzer weiterhin Probleme haben, handelt es sich höchstwahrscheinlich um **synchronisierte** Benutzer mit Verbund- oder **Kennworthash** . Dies bedeutet, dass es wahrscheinlich ein Problem mit dem Kennwortrückschreifdienst gibt.