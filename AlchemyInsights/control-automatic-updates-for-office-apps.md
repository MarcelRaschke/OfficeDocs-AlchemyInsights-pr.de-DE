---
title: Steuern automatischer Updates für Office-Apps
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 22e94d75c59e1bb0e9b5c5ce3da0be7bec9e4830
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63132509"
---
# <a name="control-automatic-updates-for-office-apps"></a>Steuern automatischer Updates für Office-Apps

Standardmäßig werden Updates für Office-Apps automatisch heruntergeladen und im Hintergrund angewendet, und zwar ohne Eingriff von Benutzern. Administratoren können jedoch mithilfe der Office-Updateeinstellungen steuern, wie Updates angewendet werden. Mithilfe der Updateeinstellungen können Administratoren automatische Updates aktivieren oder deaktivieren, die Schaltfläche **Jetzt aktualisieren** in Office ein- oder ausblenden, Updatestichtage festlegen und vieles mehr. Ausführliche Informationen finden Sie unter:

- [Konfigurieren von Updateeinstellungen für Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatische Aktualisierung für Office ist nicht aktiviert](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definieren, wie Office nach der Installation aktualisiert wird](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Um die bestehenden Updateeinstellungen zu überprüfen, die auf einen Clientcomputer angewendet werden, führen Sie diese Schritte aus:

1. Öffnen Sie den Registrierungs-Editor über **Start** > **Ausführen** > **regedit**.
2. Wechseln Sie zu folgendem Speicherort, und überprüfen Sie die Einstellungen von Office Update:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Hinweis** Wenn der OfficeMgmtCOM-Schlüssel festgelegt ist, wird unter **Office** > **Konto** > **Office-Updates** möglicherweise die Meldung "Updates werden von Ihrem Systemadministrator verwaltet" angezeigt. Weitere Informationen finden Sie unter [Verwalten von Updates für Microsoft 365 Apps mithilfe des Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  