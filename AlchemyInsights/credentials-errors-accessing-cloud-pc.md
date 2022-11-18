---
title: "\"Ihre Anmeldeinformationen haben nicht funktioniert\" oder \"Anmeldeversuch fehlgeschlagen\" beim Zugriff auf einen Cloud-PC"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010437"
- "16692"
ms.date: 02/15/2022
ms.openlocfilehash: 98ea9dcc1d2a82b0604cbb55c7b94b9c8f9f7703
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66354963"
---
# <a name="your-credentials-did-not-work-or-logon-attempt-failed-when-accessing-a-cloud-pc"></a>"Ihre Anmeldeinformationen haben nicht funktioniert" oder "Anmeldeversuch fehlgeschlagen" beim Zugriff auf einen Cloud-PC

Wenn Sie beim Versuch, sich bei einem Windows 365 Cloud-PC anzumelden, die Fehlermeldung "Ihre Anmeldeinformationen haben nicht funktioniert" oder "Anmeldeversuch fehlgeschlagen" erhalten, kann der Fehler verursacht werden, da das PKU2U-Protokoll sowohl auf dem lokalen Gerät als auch auf dem Cloud-PC nicht aktiviert ist. Weitere Informationen finden Sie unter [Netzwerksicherheit: Zulassen, dass PKU2U-Authentifizierungsanforderungen an diesen Computer Onlineidentitäten verwenden](https://docs.microsoft.com/windows/security/threat-protection/security-policy-settings/network-security-allow-pku2u-authentication-requests-to-this-computer-to-use-online-identities).

Um dieses Problem zu beheben, stellen Sie sicher, dass das PKU2U-Protokoll für den Cloud-PC auf der Registerkarte **"Konfigurationseinstellungen"** des Geräteprofils in Microsoft Endpoint Manager aktiviert ist:  

1. [Erstellen Sie einen Filter für alle Cloud-PCs](https://docs.microsoft.com/windows-365/enterprise/create-filter).
2. Erstellen Sie eine Gerätekonfigurationsrichtlinie [mithilfe des Einstellungskatalogs](https://docs.microsoft.com/mem/intune/configuration/settings-catalog).
3. Suchen Sie auf der Seite **"Konfigurationseinstellungen** " nach **PKU2U-Authentifizierungsanforderungen für Netzwerksicherheit**, und wählen Sie sie aus, und wählen Sie dann **"Zulassen"** aus.
4. Wählen Sie auf der Seite "Aufgaben" die Option **"Alle Geräte** >  hinzufügen **" den Bearbeitungsfilter** > **"Gefilterte Geräte in die Zuweisung einschließen**" und dann den Filter aus, den Sie für alle Cloud-PCs erstellt haben.
5. Schließen Sie die Erstellung der Gerätekonfigurationsrichtlinie ab.

Weitere Informationen zum Beheben von Zugriffsproblemen für Windows 365-Geräte finden Sie [unter Beheben von Cloud PC-Verbindungsfehlern](https://docs.microsoft.com/windows-365/enterprise/connection-errors).
