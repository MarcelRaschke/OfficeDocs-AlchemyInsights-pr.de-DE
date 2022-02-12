---
title: Problem beim Zurücksetzen des Kennworts
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 3968029625ed1431f70d0ee3387d016fa99c8f30
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62707857"
---
# <a name="problems-resetting-password"></a>Probleme beim Zurücksetzen des Kennworts

Es folgen einige der Probleme, die beim Zurücksetzen des Kennworts auftreten können, und die möglichen Lösungen:

**Ich habe ein Problem mit der Kennwortzurücksetzung, das in den anderen Kategorien nicht behandelt wird**

- Stellen Sie sicher, dass Sie zum Zurücksetzen von Kennwörtern autorisiert sind. Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.
- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:
    - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
        - Nur Cloudbenutzer – alle kostenpflichtigen Office 365 (O365) oder Azure AD Basic
        - Cloud- und/oder lokale Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
        - Weitere Informationen zu den Lizenzierungsanforderungen finden Sie im Artikel ["Lizenzierungsanforderungen für Azure AD Self-Service-Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)".

**Ich habe Probleme beim Testen der von mir festgelegten Kennwortzurücksetzungsrichtlinie.**

- Kürzlich angewendete Richtlinien können mehrere Minuten dauern, bis sie in allen Rechenzentren und Endpunkten repliziert wurden. Der physische Abstand zum Rechenzentrum wirkt sich auch darauf aus, wie schnell Änderungen angewendet werden.
- Testen Sie mit einem Endbenutzer, nicht mit einem Administrator, und führen Sie ein Pilotprojekt mit einer kleinen Gruppe von Benutzern durch. Die im Azure-Portal konfigurierten Richtlinien gelten NUR für Endbenutzer, nicht für Administratoren. Microsoft erzwingt für jede Azure-Administratorrolle eine starke zweistufige Kennwortzurücksetzungsrichtlinie (Beispiel: globaler Administrator, Helpdesk-Administrator, Kennwortadministrator usw.)
    - Erfahren Sie mehr über [Richtlinien für Administratoren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Ich möchte die Kennwortzurücksetzung bereitstellen, aber ich möchte meine Benutzer nicht dazu bringen, zusätzliche Sicherheitsinformationen zu registrieren.**

Füllen Sie die Daten für Ihre Benutzer vorab aus, damit sie dies nicht tun müssen! – Als Administrator können Sie Telefon- und E-Mail-Eigenschaften für Ihre Benutzer festlegen, bevor Sie die Kennwortzurücksetzung für Ihre Organisation einführen. Dazu können Sie eine API, PowerShell oder Azure AD Verbinden verwenden. Weitere Informationen:
- [Bereitstellen der Kennwortzurücksetzung, ohne dass Benutzer sich registrieren müssen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Welche Daten werden von der Kennwortzurücksetzung verwendet?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Die Schaltfläche zum Zurücksetzen des Kennworts ist abgeblendet**

Sie sind nicht berechtigt, die Kennwörter dieses Benutzers zurückzusetzen. Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das Blatt "Kennwortzurücksetzung" wird nicht angezeigt.**

Sie sind nicht berechtigt, Kennwörter zurückzusetzen. Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das lokale Integrationsblatt wird beim Zurücksetzen des Kennworts nicht angezeigt.**

- Das lokale Integrationsblatt wird nur in Hybridumgebungen angezeigt, d. h., Sie verwenden das Kennwortrückschreiben, um die Kennwörter lokaler Benutzer zu bearbeiten.
- Dieses Blatt wird nicht angezeigt, wenn:
    - Sie verwenden kein Kennwortrückschreiben
    - Es gibt ein Problem mit der Installation/Konnektivität des Kennwortrückschreibens.
    - Es liegt ein Problem bei der Installation/Konnektivität von Azure AD Verbinden
    - Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie im Abschnitt ["Problembehandlung beim Rückschreiben von Kennwörtern](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)"

**Ich weiß nicht, wie ich das Kennwort eines Benutzers zurücksetzen kann**

1. Melden Sie sich beim Azure-Portal als entsprechender Administrator an.
1. Wechseln Sie zum Blatt "Benutzer und Gruppen", und wählen Sie **"Alle Benutzer" aus**.
1. Wählen Sie einen Benutzer aus der Liste aus.
1. Wählen Sie für den ausgewählten Benutzer **die Option "Übersicht**" aus, und klicken Sie dann in der Befehlsleiste auf **"Kennwort zurücksetzen"**.
1. Folgen Sie den Anweisungen auf dem Bildschirm.
    - Nur über das Azure-Portal durchgeführte Zurücksetzungen unterstützen das Kennwortrückschreiben.

**Ich kann das Kennwort eines lokalen Benutzers aus dem Office 365 Admin-Portal oder Office 365 mobilen Anwendung zurücksetzen, aber der Benutzer kann sich immer noch nicht anmelden.**

Das Kennwortrückschreiben wird in diesem Portal nicht unterstützt. Zurücksetzen des Benutzerkennworts im Azure-Portal – portal.azure.com

