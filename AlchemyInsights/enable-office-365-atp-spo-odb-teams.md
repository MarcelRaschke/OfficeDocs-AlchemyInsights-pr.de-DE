---
title: Aktivieren Office 365 ATP für SharePoint, OneDrive und Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 3100021
ms.date: 04/21/2020
ms.openlocfilehash: 6a64f2b75086a72975fb1938a7e1ec7d8984bb97
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66421942"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Öffnen Sie unter Verwendung Ihrer Anmeldeinformationen für den globalen Administrator oder sicherheitsadministrator das Microsoft 365 Defender-Portal unter <https://security.microsoft.com>, und wechseln Sie dann im Abschnitt **"Richtlinien****" zu "Richtlinien & Regeln**\>" im Abschnitt "**Sichere Anlagen** für **Bedrohungsrichtlinien**\>".

   Um direkt zur Seite " **Sichere Anlagen"** zu wechseln, verwenden Sie <https://security.microsoft.com/safeattachmentv2>.

2. Klicken Sie auf der Seite **"Sichere Anlagen** " auf **"Globale Einstellungen"**.
3. Wählen Sie im angezeigten Flyout **"Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams aktivieren" und** dann "**Speichern"** aus.
4. (Empfohlen) Verwenden Sie als globaler Administrator oder SharePoint Online-Administrator den Wert `$true` für den *DisallowInfectedFileDownload-Parameter* im **[Cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen.
5. (Empfohlen) [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Vollständige Anweisungen finden Sie in dieser [Anleitung zum Aktivieren sicherer Anlagen für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams).

**Hinweis**: Microsoft Defender für Office 365 überprüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Weitere Informationen [finden Sie unter Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
