---
title: Aktivieren Tresor Anlagen für SharePoint Online, OneDrive und Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 64cf76c3340a4efc7d5007d63699f711fe98fc76
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62706129"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren Tresor Anlagen für SharePoint Online, OneDrive und Microsoft Teams

1. Öffnen Sie mit ihren Anmeldeinformationen für globale Administratoren oder Sicherheitsadministratoren das Microsoft 365 Defender-Portal unter <https://security.microsoft.com>, und wechseln Sie dann **im Abschnitt "****Richtlinien" zu "Richtlinien & Regeln** \> **für Bedrohungsrichtlinien** \> **Tresor Anlagen**".

   To go directly to the **Tresor Attachments** page, use <https://security.microsoft.com/safeattachmentv2>.

2. Klicken Sie auf der Seite **Tresor Anlagen** auf **globale Einstellungen**.
3. On the flyout that appears, select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams,** and then select **Save**.

    **Tipp**: Führen Sie die folgenden Schritte aus, um den Schutz von Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams zu verbessern:
    - Um zu verhindern, dass Benutzer schädliche Dateien herunterladen, verwenden Sie den Wert `$true` für den *Parameter DisallowInfectedFileDownload* im **[Cmdlet "Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)**" in SharePoint Online PowerShell. Weitere Informationen finden Sie unter [Verwenden von SharePoint Online-PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    - [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Weitere Informationen finden Sie unter [Tresor Anlagen für Office 365 für SharePoint, OneDrive und Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
