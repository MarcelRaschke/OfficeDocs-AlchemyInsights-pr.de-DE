---
title: Anwenden von Updates für Office-Apps
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
- "1747"
- "9000140"
ms.openlocfilehash: 6c09fe5befce1ff8d9b35e630b80e85a4e158356
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63285677"
---
# <a name="apply-updates-for-office-apps"></a>Anwenden von Updates für Office-Apps

Standardmäßig werden kostenlose Updates für Office-Apps automatisch heruntergeladen und im Hintergrund angewendet, und zwar ohne Eingriff von Benutzern. Wenn Sie Probleme beim Anwenden von Updates haben, finden Sie unter [Installieren von Office-Updates](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5) Informationen zum manuellen Ausführen von Updates. Weitere Informationen hierzu finden Sie unter [Problembehandlung beim Installieren von Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

Um Office-Updates für Ihre Benutzer zu verwalten, ziehen Sie diese Optionen in Betracht:

- Wählen Sie den richtigen Office-Updatekanal für Ihre Organisation auf der Grundlage der gewünschten Aktualisierungshäufigkeit aus. Weitere Informationen finden Sie unter [Übersicht über Updatekanäle für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).

- Entscheiden Sie, ob Aktualisierungen automatisch über das Internet oder über eine lokale Freigabe erfolgen sollen. Informationen dazu finden Sie unter [Auswählen, wie Updates für Microsoft 365 Apps verwaltet werden](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).

- Überprüfen Sie die Office-Updateeinstellungen, um zu steuern, wie Updates auf Endbenutzercomputer angewendet werden:

    - [Konfigurieren von Updateeinstellungen für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [Definieren, wie Office nach der Installation aktualisiert wird](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).

Wenn Sie Office-Apps für mehrere Benutzer bereitstellen, verwenden Sie das Office-Anpassungstool, um Konfigurationsdateien für die Bereitstellung zu erstellen, und konfigurieren Sie Office-Updates mithilfe des Office-Bereitstellungstools. Weitere Informationen finden Sie unter [Übersicht über das Office-Anpassungstool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) und das [Office-Bereitstellungstool](https://go.microsoft.com/fwlink/p/?LinkID=626065).

- Ein Beispiel für die Einrichtung von Benutzergruppen zur Bereitstellung von Office-Updates finden Sie unter [Bereitstellen von Microsoft 365 Apps aus einer lokalen Quelle](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).
-   Ziehen Sie in Betracht, die Einstellung "ForceAppShutdown" zu verwenden, falls Office-Updates aufgrund geöffneter Office-Apps bei einigen Benutzern nicht angewendet werden. Weitere Informationen finden Sie in der [FORCEAPPSHUTDOWN-Eigenschaft (Teil des Property-Elements)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element). 

**Siehe auch**

[Übersicht über den Updateprozess für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Versionsinformationen zu Updates für Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).  
[Verwalten von Updates für Microsoft 365 Apps mithilfe von Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).  
