---
title: Aktivieren Office 365 ATP für SharePoint, OneDrive und Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 1e5145a7c729742f4f5c3421ec9c4a8995db4e46
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62747531"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Öffnen Sie mit ihren Anmeldeinformationen für globale Administratoren oder Sicherheitsadministratoren das Microsoft 365 Defender Portal unter <https://security.microsoft.com>, und wechseln Sie dann **im Abschnitt "****Richtlinien" zu Richtlinien & Regeln** \> **für Bedrohungsrichtlinien** \> **Tresor Anlagen**.

   To go directly to the **Tresor Attachments** page, use <https://security.microsoft.com/safeattachmentv2>.

2. Klicken Sie auf der Seite **Tresor Anlagen** auf **globale Einstellungen**.
3. On the flyout that appears, select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams,** and then select **Save**.
4. (Empfohlen) Verwenden Sie als globaler Administrator oder SharePoint Onlineadministrator den Wert `$true` für den *Parameter DisallowInfectedFileDownload* im Cmdlet **["Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)**" in SharePoint Online PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen.
5. (Empfohlen) [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Vollständige Anweisungen finden Sie unter "[Aktivieren Tresor Anlagen für SharePoint,OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)".

**Hinweis**: Microsoft Defender für Office 365 überprüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Informationen [zu SharePoint, OneDrive und Microsoft Teams finden Sie unter Microsoft Defender für Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
