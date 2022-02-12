---
title: Probleme mit Anmeldeinformationen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: f8579cf9e4c023c22a9c5d2ee5312e98898b4a00
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62590546"
---
# <a name="issues-with-credentials"></a>Probleme mit Anmeldeinformationen

[Microsoft Identity Platform und der OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beschreibt, wie sie direkt mit dem Fluss zur Gewährung von OAuth 2.0-Clientanmeldeinformationen programmieren.

**Wie verwalte ich das Kennwort oder die Zertifikatanmeldeinformationen einer Anwendung?**

In der Azure CLI können Sie [az ad app-Anmeldeinformationen](https://docs.microsoft.com/cli/azure/ad/app/credential) verwenden, um das Kennwort oder die Zertifikatanmeldeinformationen einer Anwendung zu löschen, aufzuführen oder zurückzusetzen.

**Wie können meine Benutzer ihre Kennwörter zurücksetzen?**

Benutzer müssen [sich für die Self-Service-Kennwortzurücksetzung registrieren](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) , bevor sie ihre Kennwörter zurücksetzen können. Nachdem sich ein Benutzer registriert hat, kann er den Anweisungen in diesem Artikel folgen, um sein Kennwort zurückzusetzen: [Zurücksetzen Ihres Geschäfts-, Schul- oder Unikennworts](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Wie können meine Benutzer ihre Kennwörter ändern?**

Benutzer können die Schritte in diesem Artikel ausführen, um ihre Kennwörter zu ändern: [So ändern Sie Ihr Kennwort](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Sie können auch [App-Kennwörter für die zweistufige Überprüfung verwalten](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Mein Benutzer erhält einen Fehler beim Ändern oder Zurücksetzen des Kennworts**

Dieser Link enthält Informationen zu allgemeinen Problemen, die auftreten können, wenn ein Benutzer versucht, sein Kennwort zurückzusetzen: [häufige Probleme und lösungen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Ich habe ein Problem beim Zurücksetzen des Kennworts eines Benutzers**

- Stellen Sie sicher, dass Sie berechtigt sind, Kennwörter zurückzusetzen. *Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:

  - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein:
    - **Nur Cloudbenutzer** – alle kostenpflichtigen Office 365 (O365) oder Azure AD Basic
    - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu den Lizenzierungsanforderungen finden Sie unter ["Lizenzierungsanforderungen für Azure AD Self-Service-Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)".
- Um das Kennwort eines Benutzers zurückzusetzen, suchen Sie den Benutzer in Azure AD. Klicken Sie dann auf dem Blatt "Übersicht" für diesen Benutzer auf die Schaltfläche "Kennwort zurücksetzen".

**Die Schaltfläche zum Zurücksetzen des Kennworts ist abgeblendet**

Sie sind nicht berechtigt, die Kennwörter **dieses** Benutzers zurückzusetzen. *Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das Blatt "Kennwortzurücksetzung" wird nicht angezeigt.**

Sie sind nicht berechtigt, Kennwörter zurückzusetzen. *Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das lokale Integrationsblatt wird beim Zurücksetzen des Kennworts nicht angezeigt.**

- Das lokale Integrationsblatt wird nur in Hybridumgebungen angezeigt, d. h., Sie verwenden das Kennwortrückschreiben, um die Kennwörter lokaler Benutzer zu bearbeiten.

- Dieses Blatt wird nicht angezeigt, wenn:

  - Sie verwenden kein Kennwortrückschreiben
  - Es gibt ein Problem mit der Installation/Konnektivität des Kennwortrückschreibens.
  - Es gibt ein Problem mit der Installation/Konnektivität von Azure AD Verbinden
  - Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie unter [Problembehandlung beim Kennwortrückschreiben](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback).

**Ich weiß nicht, wie ich das Kennwort eines Benutzers zurücksetzen kann**

1. Melden Sie sich beim Azure-Portal als entsprechender Administrator an.
2. Wechseln Sie zum Blatt **"Benutzer und Gruppen** ", und wählen Sie **"Alle Benutzer" aus**.
3. Wählen Sie einen Benutzer aus der Liste aus.
4. Wählen Sie für den ausgewählten Benutzer **"Übersicht**" und dann in der Befehlsleiste " **Kennwort zurücksetzen**" aus.
5. Wählen Sie die Schaltfläche **"Kennwort zurücksetzen** " aus, und folgen Sie den Anweisungen auf dem Bildschirm.
    - Nur über das **Azure-Portal** durchgeführte Zurücksetzungen unterstützen das Kennwortrückschreiben.

**Ich kann das Kennwort eines lokalen Benutzers aus dem Office 365 Admin-Portal oder Office 365 mobilen Anwendung zurücksetzen, aber der Benutzer kann sich immer noch nicht anmelden.**

Das Kennwortrückschreiben wird in diesem Portal nicht unterstützt. Setzen Sie das Kennwort des Benutzers im Azure-Portal erneut zurück.
