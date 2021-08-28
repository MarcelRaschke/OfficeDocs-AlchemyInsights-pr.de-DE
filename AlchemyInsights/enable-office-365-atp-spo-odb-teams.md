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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332158"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Wechseln Sie zu https://protection.office.com, und melden Sie sich an.
2. Wählen Sie Die Richtlinie für **die Bedrohungsverwaltung**  >    >  **Tresor Anlagen aus.**
3. Wählen Sie **"Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams** aktivieren" aus, und klicken Sie dann auf **"Speichern".**
4. (Empfohlen) Führen Sie als globaler Administrator oder SharePoint Onlineadministrator das Cmdlet ["Set-SPOTenant"](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) aus, wobei der **Parameter "DisallowInfectedFileDownload"** auf *"true"* festgelegt ist.
5. (Empfohlen) [Richten Sie Warnungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien ein.

**Hinweis:** Microsoft Defender für Office 365 überprüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Informationen [zu SharePoint, OneDrive und Microsoft Teams finden Sie unter Microsoft Defender für Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
