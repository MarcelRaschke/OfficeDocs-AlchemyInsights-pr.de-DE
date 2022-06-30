---
title: Aktivieren sicherer Anlagen für SharePoint Online, OneDrive und Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ddcfa5853cb2ba636806f75ecd619887fb2948e2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66394275"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren sicherer Anlagen für SharePoint Online, OneDrive und Microsoft Teams

1. Öffnen Sie unter Verwendung Ihrer Anmeldeinformationen für den globalen Administrator oder Sicherheitsadministrator das Microsoft 365 Defender Portal unter <https://security.microsoft.com>, und wechseln Sie dann im Abschnitt "**Richtlinien" zu "Richtlinien & Regeln**\>" im Abschnitt "Richtlinien" zu **"Bedrohungsrichtlinien** \> **für sichere Anlagen**".

   Um direkt zur Seite " **Sichere Anlagen"** zu wechseln, verwenden Sie <https://security.microsoft.com/safeattachmentv2>.

2. Klicken Sie auf der Seite **"Sichere Anlagen** " auf **"Globale Einstellungen"**.
3. Wählen Sie im angezeigten Flyout **"Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams aktivieren" und** dann "**Speichern"** aus.

    **Tipp**: Führen Sie die folgenden Schritte aus, um den Schutz sicherer Anlagen für SharePoint, OneDrive und Microsoft Teams zu verbessern:
    - Um zu verhindern, dass Benutzer schädliche Dateien herunterladen, verwenden Sie den Wert `$true` für den *DisallowInfectedFileDownload-Parameter* im **[Cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell. Weitere Informationen finden Sie unter [Verwenden von SharePoint Online PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    - [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Weitere Informationen finden Sie unter ["Sichere Anlagen" für Office 365 für SharePoint, OneDrive und Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
