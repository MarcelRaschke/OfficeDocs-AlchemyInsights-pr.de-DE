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
ms.openlocfilehash: f6e39ac25ef3fc9bb05b0d07ab66ebf6e1a0b80f
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799974"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Öffnen Sie mit ihren Anmeldeinformationen für globale Administratoren oder Sicherheitsadministratoren das Microsoft 365 Defender Portal unter , und wechseln Sie <https://security.microsoft.com> dann im Abschnitt **"Richtlinien" zu "Richtlinien & Regeln** für \> **Bedrohungsrichtlinien** Tresor \> **Anlagen".** 

   To go directly to the **Tresor Attachments** page, use <https://security.microsoft.com/safeattachmentv2> .

2. Klicken Sie auf der Seite **Tresor Anlagen** auf **globale Einstellungen.**
3. Wählen Sie im angezeigten Flyout **Microsoft Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams** aktivieren und dann **speichern** aus.
4. (Empfohlen) Verwenden Sie als globaler Administrator oder SharePoint Onlineadministrator den Wert `$true` für den *Parameter "DisallowInfectedFileDownload"* im Cmdlet **["Set-SPOTenant"](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell, um zu verhindern, dass Benutzer schädliche Dateien herunterladen.
5. (Empfohlen) [Erstellen einer Warnungsrichtlinie für erkannte Dateien](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Vollständige Anweisungen finden Sie unter dieser [Option zum Aktivieren von Tresor Anlagen für SharePoint, OneDrive und Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)

**Hinweis:** Microsoft Defender für Office 365 überprüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Informationen [zu SharePoint, OneDrive und Microsoft Teams finden Sie unter Microsoft Defender für Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
