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
ms.localizationpriority: medium
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 9f3313f615d6c375aa2fdc265bc3d30f61b135c5
ms.sourcegitcommit: 9edb4aa99886a74c1f391d1927d5f8d16d6b6904
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65551925"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Öffnen Sie unter Verwendung Ihrer Anmeldeinformationen für den globalen Administrator oder Sicherheitsadministrator das Microsoft 365 Defender Portal unter <https://security.microsoft.com>, und wechseln Sie dann im Abschnitt **"Richtlinien****" zu "Richtlinien & Regeln** \> **" für Bedrohungsrichtlinien** \> **Tresor Anlagen**.

   Um direkt zur Seite **Tresor Anlagen** zu wechseln, verwenden Sie <https://security.microsoft.com/safeattachmentv2>.

2. Klicken Sie auf der Seite **Tresor Anlagen** auf **"Globale Einstellungen"**.
3. Wählen Sie im angezeigten Flyout **"Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams aktivieren**" und dann "**Speichern"** aus.
4. (Empfohlen) Verwenden Sie als globaler Administrator oder SharePoint Onlineadministrator den Wert `$true` für den Parameter *DisallowInfectedFileDownload* im Cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen.
5. (Empfohlen) [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Vollständige Anweisungen finden Sie in diesem [Thema zum Aktivieren Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams).

**Hinweis**: Microsoft Defender für Office 365 überprüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Informationen [zu SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams) finden Sie Microsoft Defender für Office 365.
