---
title: "\"Ihre Anmeldeinformationen haben nicht funktioniert\" oder \"Anmeldeversuch fehlgeschlagen\" beim Zugriff auf einen Cloud-PC"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9010437"
- "16692"
ms.date: 02/15/2022
ms.openlocfilehash: 28d7cbaf25e3b6dcff11d3a42d29c6501b93364c
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63278117"
---
# <a name="your-credentials-did-not-work-or-logon-attempt-failed-when-accessing-a-cloud-pc"></a>"Ihre Anmeldeinformationen haben nicht funktioniert" oder "Anmeldeversuch fehlgeschlagen" beim Zugriff auf einen Cloud-PC

Wenn Sie beim Versuch, sich bei einem Windows 365 Cloud-PC anzumelden, Fehler "Ihre Anmeldeinformationen haben nicht funktioniert" oder "Anmeldeversuch fehlgeschlagen" erhalten, kann der Fehler verursacht werden, da das PKU2U-Protokoll auf dem lokalen Gerät und dem Cloud-PC nicht aktiviert ist. Weitere Informationen finden Sie unter ["Netzwerksicherheit: Zulassen der Verwendung von Onlineidentitäten durch PKU2U-Authentifizierungsanforderungen an diesen Computer](https://docs.microsoft.com/windows/security/threat-protection/security-policy-settings/network-security-allow-pku2u-authentication-requests-to-this-computer-to-use-online-identities)".

Um dieses Problem zu beheben, stellen Sie sicher, dass das PKU2U-Protokoll für den Cloud-PC auf der Registerkarte " **Konfigurationseinstellungen** " des Geräteprofils in Microsoft Endpoint Manager aktiviert ist:  

1. [Erstellen Sie einen Filter für alle Cloud-PCs](https://docs.microsoft.com/windows-365/enterprise/create-filter).
2. Erstellen Sie eine Gerätekonfigurationsrichtlinie [mithilfe des Einstellungskatalogs](https://docs.microsoft.com/mem/intune/configuration/settings-catalog).
3. Suchen Sie auf der Seite **"Konfigurationseinstellungen** " nach **"PKU2U-Authentifizierungsanforderungen für Netzwerksicherheit zulassen"**, und wählen Sie sie aus, und wählen Sie dann " **Zulassen**" aus.
4. Wählen Sie auf der Seite **"Aufgaben**" **die Option "Alle Geräte** >  **hinzufügenEdit filterInclude** >  **gefilterte Geräte in Der Zuweisung** hinzufügen" aus, und wählen Sie dann den Filter aus, den Sie für alle Cloud-PCs erstellt haben.
5. Schließen Sie die Erstellung der Gerätekonfigurationsrichtlinie ab.

Weitere Informationen zum Beheben von Zugriffsproblemen für Windows 365-Geräte finden Sie unter [Problembehandlung von Cloud-PC-Verbindungsfehlern](https://docs.microsoft.com/windows-365/enterprise/connection-errors).
