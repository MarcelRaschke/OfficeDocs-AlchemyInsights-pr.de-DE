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
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 0871b3f139e98f6d2e67a68b57aab6b6902694e4
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799902"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams

Führen Sie die folgenden Schritte aus:

1. Öffnen Sie mit ihren Anmeldeinformationen für globale Administratoren oder Sicherheitsadministratoren das portal Microsoft 365 Defender unter , und wechseln Sie <https://security.microsoft.com> dann im Abschnitt **"Richtlinien" zu "Richtlinien & Regeln** für \> **Bedrohungsrichtlinien** Tresor \> **Anlagen".** 

   To go directly to the **Tresor Attachments** page, use <https://security.microsoft.com/safeattachmentv2> .

2. Klicken Sie auf der Seite **Tresor Anlagen** auf **globale Einstellungen.**
3. Wählen Sie im angezeigten Flyout **Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams** aktivieren und dann **speichern** aus.

    **Tipp:** Führen Sie die folgenden Schritte aus, um den Schutz von Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams zu verbessern:
    - Um zu verhindern, dass Benutzer schädliche Dateien herunterladen, verwenden Sie den Wert `$true` für den *Parameter DisallowInfectedFileDownload* im **[Cmdlet "Set-SPOTenant"](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell. Weitere Informationen finden Sie unter [Verwenden von SharePoint Online-PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Vollständige Anweisungen finden Sie unter dieser [Option zum Aktivieren von Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)

**Hinweis:** Standardmäßig überprüft Microsoft Defender für Office 365 nicht jede einzelne Datei in SharePoint Online, OneDrive for Business oder Microsoft Teams. Dateien werden asynchron von einem Prozess gescannt, der Freigabeaktivitäten, Gastaktivitäten und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Weitere Informationen finden Sie unter [Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
