---
title: Installieren von Office auf einem Terminalserver – Nicht lizenziert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: f1b165fa3d0c19de74d4a579ee8a70dc776962da
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63127715"
---
# <a name="installing-office-on-a-terminal-server"></a>Installieren von Office auf einem Terminalserver

Für die Bereitstellung von Microsoft 365 Apps for Enterprise auf einem Windows Server mitHilfe von Remotedesktopdiensten (RDS), früher terminal services genannt:
  
- Sie müssen über ein Microsoft 365-Abonnement verfügen, das Microsoft 365 Apps for Enterprise umfasst, z. B. Office 365 Enterprise E3 oder Enterprise E5. Die Pläne "Microsoft 365 Apps for Business" und "Microsoft 365 Apps for Business Premium" enthalten nicht Microsoft 365 Apps for Enterprise.

- Sie müssen die [Aktivierung freigegebener Computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation) aktivieren.

Wenn Sie Microsoft 365 Apps for Enterprise auf RDS über das Microsoft 365 Admin Center installieren möchten, ***das standardmäßige Installationseinstellungen verwendet***, führen Sie die folgenden Schritte aus.

**Tipp**: Sie können auch den [Microsoft-Support- und Wiederherstellungs-Assistenten herunterladen und](https://aka.ms/SaRA_OfficeSCA_M365Portal) ausführen, um Microsoft 365 Apps for Enterprise im Aktivierungsmodus für gemeinsam genutzte Computer zu installieren.
  
1. Überprüfen Sie, über welches Microsoft 365-Abonnement Sie verfügen. [Anleitung](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Wechseln Sie bei Bedarf zu einem anderen Microsoft 365-Abonnement. [Anleitung](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Wenn Office bereits auf dem RDS-Server mit anderen Microsoft 365-Abonnements installiert ist, deinstallieren Sie es. Gehen Sie beispielsweise zur Systemsteuerung \> , um ein Programm zu deinstallieren. Deinstallieren Sie den [Microsoft-Support- und Wiederherstellungs-Assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) , wenn Probleme auftreten.

4. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Microsoft 365 Admin Center an, und [installieren Sie Microsoft 365 Apps for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Öffnen sie nach der Installation von Office keine Office-Anwendungen ***, und melden Sie sich nicht*** an.

6. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer, indem Sie die Registrierung wie folgt bearbeiten:

1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie "Ausführen" aus. Geben Sie im Feld "Öffnen" **"regedit**" ein, und wählen Sie dann "OK" aus.

2. Wählen Sie "Ja" aus, wenn Sie aufgefordert werden, dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu erlauben.

3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration hinzu.

7. ***Melden Sie sich*** auf dem RDS-Server als Endbenutzer an, und [stellen Sie sicher, dass die Aktivierung freigegebener Computer für Microsoft 365 Apps for Enterprise aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Weitere Informationen zu den Voraussetzungen, Setupanweisungen und Anleitungen zu angepassten Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Bereitstellen von Microsoft 365 Apps for Enterprise mithilfe von Remotedesktopdiensten](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Problembehandlung bei der Aktivierung freigegebener Computer für Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  