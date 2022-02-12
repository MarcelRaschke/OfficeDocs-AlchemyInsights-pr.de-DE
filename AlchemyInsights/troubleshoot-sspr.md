---
title: Problembehandlung bei SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: d3fc8e81fd4508866df99ec9e70446a74d6de4f6
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62645880"
---
# <a name="troubleshoot-sspr"></a>Problembehandlung bei SSPR

**Ich habe Probleme beim Konfigurieren der Kennwortzurücksetzung**

- Wenn Sie Administrator sind und nach der Möglichkeit suchen, die Self-Service-Kennwortzurücksetzung zu aktivieren, lesen [Sie Lernprogramm zum Aktivieren von SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), um die Kennwortzurücksetzung für Ihre Organisation zu konfigurieren. Möglicherweise möchten Sie auch die [Lizenzierungsanforderungen](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) überprüfen. Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
    - **Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365) oder Azure AD Basic
    - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
- Weitere Fragen zur Self-Service-Kennwortzurücksetzung finden Sie in [unseren häufig gestellten Fragen](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ich erhalte eine Fehlermeldung**

Lesen Sie diesen Artikel, um häufige Fehler und deren Lösungen zu finden: [Problembehandlung beim Zurücksetzen von Self-Service-Kennwörtern](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich habe ein Problem mit meiner Kennwortzurücksetzungsrichtlinie**

- Wenn sich Ihre Kennwortzurücksetzungsrichtlinie nicht wie erwartet verhält oder Sie Fragen zu Richtlinien für die Kennwortzurücksetzung haben, lesen Sie diesen Artikel: [Kennwortrichtlinien und Einschränkungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Richtlinien für die Kennwortzurücksetzung gelten nicht für Administratoren. Microsoft erzwingt für jede Azure-Administratorrolle eine starke zweistufige Kennwortzurücksetzungsrichtlinie. Stellen Sie sicher, dass Sie Tests mit einem Benutzer durchführen, der kein Administrator ist. Weitere Informationen zur Richtlinie zum Zurücksetzen von Administratoren finden Sie in diesem Artikel: [Richtlinienunterschiede beim Zurücksetzen von Administratoren](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Ich möchte nicht, dass meine Benutzer zusätzliche Sicherheitsinformationen für die Kennwortzurücksetzung registrieren.**

Sie können Daten (E-Mail- und Telefonattribute) für Ihre Benutzer vorab mithilfe einer API, PowerShell oder Azure AD Verbinden auffüllen. So erfahren Sie, wie Sie lesen:

- [Bereitstellen der Kennwortzurücksetzung, ohne dass Benutzer sich registrieren müssen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Welche Daten werden von der Kennwortzurücksetzung verwendet?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich möchte, dass meine Benutzer ihre zusätzlichen Sicherheitsinformationen für die Kennwortzurücksetzung registrieren.**

1. Lassen Sie Ihre Benutzer ihre Sicherheitsinformationen für die Self-Service-Kennwortzurücksetzung registrieren, indem Sie sie an [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info) weiterleiten.
1. Nachdem die Daten für den Benutzer (vom Benutzer oder vom Administrator) aufgefüllt wurden, leiten Sie Ihren Benutzer zu [aka.ms/sspr](https://passwordreset.microsoftonline.com/) , damit Ihre Benutzer ihre eigenen Kennwörter zurücksetzen können.
1. Wenn bei Benutzern weiterhin Probleme auftreten, handelt es sich höchstwahrscheinlich um Benutzer mit **Verbund** - oder **Kennworthashsynched** . Dies bedeutet, dass es wahrscheinlich ein Problem mit dem Kennwortrückschreibdienst gibt.