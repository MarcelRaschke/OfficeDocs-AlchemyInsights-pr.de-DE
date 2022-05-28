---
title: Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d30429cd77ec9d39e3a3220ca10c436b795238c
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65725189"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams

Führen Sie die folgenden Schritte aus:

1. Öffnen Sie unter Verwendung Ihrer Anmeldeinformationen für den globalen Administrator oder Sicherheitsadministrator das Microsoft 365 Defender Portal unter <https://security.microsoft.com>, und wechseln Sie dann im Abschnitt "**Richtlinien" zu "Richtlinien & Regeln** \> **Bedrohungsrichtlinien** \> **Tresor Anlagen****"**.

   Um direkt zur Seite **Tresor Anlagen** zu wechseln, verwenden Sie <https://security.microsoft.com/safeattachmentv2>.

2. Klicken Sie auf der Seite **Tresor Anlagen** auf **"Globale Einstellungen"**.
3. Wählen Sie im angezeigten Flyout **"Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams aktivieren**" und dann "**Speichern"** aus.

    **Tipp**: Führen Sie die folgenden Schritte aus, um den Schutz von Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams zu verbessern:
    - Um zu verhindern, dass Benutzer schädliche Dateien herunterladen, verwenden Sie den Wert `$true` für den *DisallowInfectedFileDownload-Parameter* im **[Cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell. Weitere Informationen finden Sie unter [Verwenden von SharePoint Online PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    - [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Vollständige Anweisungen finden Sie in diesem [Thema zum Aktivieren Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams).

**Hinweis**: Standardmäßig überprüft Microsoft Defender für Office 365 nicht jede einzelne Datei in SharePoint Online, OneDrive for Business oder Microsoft Teams. Dateien werden asynchron von einem Prozess gescannt, der Freigabeaktivitäten, Gastaktivitäten und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Weitere Informationen finden Sie [unter Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
