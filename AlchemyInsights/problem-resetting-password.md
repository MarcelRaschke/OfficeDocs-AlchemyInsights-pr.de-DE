---
title: Problem beim Zurücksetzen des Kennworts
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003259"
- "9360"
ms.date: 03/09/2021
ms.openlocfilehash: ddb427f06ad6a3f8efbea6728ea0bd3519470c7d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66374079"
---
# <a name="problems-resetting-password"></a>Probleme beim Zurücksetzen des Kennworts

Es folgen einige der Probleme, mit denen Sie beim Zurücksetzen des Kennworts konfrontiert sein könnten, und die möglichen Lösungen:

**Ich habe ein Problem mit der Kennwortzurücksetzung, das in den anderen Kategorien nicht behandelt wird**

- Stellen Sie sicher, dass Sie berechtigt sind, Kennwörter zurückzusetzen. Nur globale Administratoren, Kennwortadministratoren und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.
- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:
    - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
        - Nur Cloudbenutzer – alle Office 365 (O365) kostenpflichtige SKU oder Azure AD Basic
        - Cloud- und/oder lokale Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
        - Weitere Informationen zu den Lizenzierungsanforderungen finden Sie im Artikel [Lizenzierungsanforderungen für die Self-Service-Kennwortzurücksetzung von Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ich habe Probleme beim Testen der kennwortzurücksetzungsrichtlinie, die ich festgelegt habe**

- Zuletzt angewendete Richtlinien können mehrere Minuten dauern, bis sie in allen Rechenzentren und Endpunkten repliziert werden. Die physische Entfernung vom Rechenzentrum wirkt sich auch darauf aus, wie schnell Änderungen angewendet werden.
- Testen Sie mit einem Endbenutzer, nicht einem Administrator, und führen Sie ein Pilotprojekt mit einer kleinen Gruppe von Benutzern durch. Die im Azure-Portal konfigurierten Richtlinien gelten NUR für Endbenutzer, nicht für Administratoren. Microsoft erzwingt eine starke Zwei-Tor-Kennwortzurücksetzungsrichtlinie für jede Azure-Administratorrolle (Beispiel: Globaler Administrator, Helpdesk-Administrator, Kennwortadministrator usw.).
    - Erfahren Sie mehr über [Richtlinien für Administratoren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Ich möchte die Kennwortzurücksetzung bereitstellen, aber ich möchte nicht, dass meine Benutzer zusätzliche Sicherheitsinformationen registrieren.**

Füllen Sie Vorabdaten für Ihre Benutzer aus, damit sie sie nicht benötigen! – Als Administrator können Sie Telefon- und E-Mail-Eigenschaften für Ihre Benutzer festlegen, bevor Sie die Kennwortzurücksetzung für Ihre Organisation einführen. Dazu können Sie eine API, PowerShell oder Azure AD Connect verwenden. Weitere Informationen hier:
- [Bereitstellen der Kennwortzurücksetzung, ohne dass Benutzer sich registrieren müssen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Welche Daten werden von der Kennwortzurücksetzung verwendet?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Die Schaltfläche zum Zurücksetzen des Kennworts ist abgeblendet.**

Sie sind nicht berechtigt, die Kennwörter dieses Benutzers zurückzusetzen. Nur globale Administratoren, Kennwortadministratoren und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das Kennwortzurücksetzungsblatt wird nicht angezeigt.**

Sie sind nicht berechtigt, Kennwörter zurückzusetzen. Nur globale Administratoren, Kennwortadministratoren und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das lokale Integrationsblatt wird bei der Kennwortzurücksetzung nicht angezeigt.**

- Das lokale Integrationsblatt wird nur in Hybridumgebungen angezeigt, d. h., Sie verwenden das Kennwortrückschreiben, um die Kennwörter des lokalen Benutzers zu bearbeiten.
- Dieses Blatt wird nicht angezeigt, wenn:
    - Sie verwenden kein Kennwortrückschreiben
    - Problem bei der Installation/Konnektivität des Kennwortrückschreibens
    - Es besteht ein Problem bei der Installation/Konnektivität von Azure AD Connect.
    - Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie im Abschnitt ["Problembehandlung beim Kennwortrückschreiben](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)".

**Ich weiß nicht, wie ich das Kennwort eines Benutzers zurücksetzt**

1. Melden Sie sich bei der Azure-Portal als geeigneter Administrator an.
1. Wechseln Sie zum Blatt "Benutzer und Gruppen", und wählen Sie **"Alle Benutzer**" aus.
1. Wählen Sie einen Benutzer aus der Liste aus.
1. Wählen Sie für den ausgewählten Benutzer " **Übersicht**" aus, und klicken Sie dann in der Befehlsleiste auf **"Kennwort zurücksetzen"**.
1. Folgen Sie den Anweisungen auf dem Bildschirm.
    - Es werden nur Rücksetzungen durchgeführt, die über die Azure-Portal Kennwortrückschreibung unterstützt werden.

**Ich habe das Kennwort eines lokalen Benutzers über das Office 365 Admin Portal oder Office 365 mobile Anwendung zurückgesetzt, aber der Benutzer kann sich immer noch nicht anmelden.**

Das Kennwortrückschreiben wird in diesem Portal nicht unterstützt. Zurücksetzen des Benutzerkennworts im Azure-Portal – portal.azure.com

