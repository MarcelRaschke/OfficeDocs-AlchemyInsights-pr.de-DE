---
title: Probleme mit Anmeldeinformationen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 82c1fb0af5e581e8363389c839639705ea221318
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66295903"
---
# <a name="issues-with-credentials"></a>Probleme mit Anmeldeinformationen

[Microsoft Identity Platform und der OAuth 2.0-Clientanmeldeinformationenfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beschreibt, wie Sie direkt mit dem Fluss zur Gewährung von OAuth 2.0-Clientanmeldeinformationen programmieren.

**Gewusst wie das Kennwort oder die Zertifikatanmeldeinformationen einer Anwendung verwalten?**

In der Azure CLI können Sie [az ad-App-Anmeldeinformationen](https://docs.microsoft.com/cli/azure/ad/app/credential) verwenden, um das Kennwort oder die Zertifikatanmeldeinformationen einer Anwendung zu löschen, auflisten oder zurücksetzen.

**Wie können meine Benutzer ihre Kennwörter zurücksetzen?**

Benutzer müssen [sich für die Self-Service-Kennwortzurücksetzung registrieren](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) , bevor sie ihre Kennwörter zurücksetzen können. Nachdem sich ein Benutzer registriert hat, kann er den Anweisungen in diesem Artikel folgen, um sein Kennwort zurückzusetzen: [Setzen Sie Ihr Geschäfts-, Schul- oder Unikennwort zurück](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Wie können meine Benutzer ihre Kennwörter ändern?**

Benutzer können die Schritte in diesem Artikel ausführen, um ihre Kennwörter zu ändern: [So ändern Sie Ihr Kennwort](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Sie können auch [App-Kennwörter für die Überprüfung in zwei Schritten verwalten](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Mein Benutzer erhält eine Fehlermeldung beim Ändern oder Zurücksetzen seines Kennworts.**

Dieser Link enthält Informationen zu häufig auftretenden Problemen, die auftreten können, wenn ein Benutzer versucht, sein Kennwort zurückzusetzen: [Häufige Probleme und ihre Lösungen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Ich habe ein Problem beim Zurücksetzen des Kennworts eines Benutzers**

- Stellen Sie sicher, dass Sie berechtigt sind, Kennwörter zurückzusetzen. *Nur globale Administratoren, Kennwortadministratoren und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

- Stellen Sie sicher, dass Sie mit den Lizenzierungsanforderungen vertraut sind:

  - In Ihrer Organisation muss mindestens eine Lizenz zugewiesen sein:
    - **Nur Cloudbenutzer** – alle Office 365 (O365) kostenpflichtige SKU oder Azure AD Basic
    - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu Lizenzierungsanforderungen finden Sie unter [Lizenzierungsanforderungen für die Self-Service-Kennwortzurücksetzung in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Um das Kennwort eines Benutzers zurückzusetzen, suchen Sie den Benutzer in Azure AD. Klicken Sie dann auf dem Blatt "Übersicht" für diesen Benutzer auf die Schaltfläche "Kennwort zurücksetzen".

**Die Schaltfläche zum Zurücksetzen des Kennworts ist abgeblendet.**

Sie sind nicht berechtigt, die Kennwörter **dieses** Benutzers zurückzusetzen. *Nur globale Administratoren, Kennwortadministratoren und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das Kennwortzurücksetzungsblatt wird nicht angezeigt.**

Sie sind nicht berechtigt, Kennwörter zurückzusetzen. *Nur globale Administratoren, Kennwortadministratoren und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das lokale Integrationsblatt wird bei der Kennwortzurücksetzung nicht angezeigt.**

- Das lokale Integrationsblatt wird nur in Hybridumgebungen angezeigt, d. h., Sie verwenden das Kennwortrückschreiben, um die Kennwörter des lokalen Benutzers zu bearbeiten.

- Dieses Blatt wird nicht angezeigt, wenn:

  - Sie verwenden kein Kennwortrückschreiben
  - Problem bei der Installation/Konnektivität des Kennwortrückschreibens
  - Es besteht ein Problem bei der Installation/Konnektivität von Azure AD Connect.
  - Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie [unter Problembehandlung beim Kennwortrückschreiben](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ich weiß nicht, wie ich das Kennwort eines Benutzers zurücksetzt**

1. Melden Sie sich bei der Azure-Portal als geeigneter Administrator an.
2. Wechseln Sie zum Blatt **"Benutzer und Gruppen** ", und wählen Sie **"Alle Benutzer**" aus.
3. Wählen Sie einen Benutzer aus der Liste aus.
4. Wählen Sie für den ausgewählten Benutzer **"Übersicht**" und dann in der Befehlsleiste " **Kennwort zurücksetzen"** aus.
5. Wählen Sie die Schaltfläche " **Kennwort zurücksetzen** " aus, und folgen Sie den Anweisungen auf dem Bildschirm.
    - Es werden nur Rücksetzungen durchgeführt, die über die **Azure-Portal** Kennwortrückschreibung unterstützt werden.

**Ich habe das Kennwort eines lokalen Benutzers über das Office 365 Admin Portal oder Office 365 mobile Anwendung zurückgesetzt, aber der Benutzer kann sich immer noch nicht anmelden.**

Das Kennwortrückschreiben wird in diesem Portal nicht unterstützt. Setzen Sie das Kennwort des Benutzers im Azure-Portal erneut zurück.
