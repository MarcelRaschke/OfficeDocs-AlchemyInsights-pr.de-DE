---
title: Installieren von Office auf einem Terminalserver – Nicht lizenziert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321998"
---
# <a name="installing-office-on-a-terminal-server"></a>Installieren von Office auf einem Terminalserver

Für die Bereitstellung von Microsoft 365 Apps for Enterprise auf einem Windows Server mitHilfe von Remotedesktopdiensten (RDS), früher Terminaldienste genannt:
  
- Sie müssen über ein Microsoft 365 Abonnement verfügen, das Microsoft 365 Apps for Enterprise enthält, z. B. Office 365 Enterprise E3 oder Enterprise E5. Die Pläne für Microsoft 365 Apps for Business und Microsoft 365 Apps for Business Premium enthalten keine Microsoft 365 Apps for Enterprise.

- Sie müssen die [Aktivierung freigegebener Computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)aktivieren.

Wenn Sie Microsoft 365 Apps for Enterprise auf RDS aus dem Microsoft 365 Admin Center installieren möchten, ***das die Standardinstallationseinstellungen verwendet,*** führen Sie die folgenden Schritte aus.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Überprüfen Sie, über welches Microsoft 365 Abonnement Sie verfügen. [Anleitung](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Wechseln Sie bei Bedarf zu einem anderen Microsoft 365 Abonnement. [Anleitung](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Wenn Office bereits auf dem RDS-Server mit anderen Microsoft 365-Abonnements installiert ist, deinstallieren Sie es. Gehen Sie beispielsweise zur Systemsteuerung, um ein Programm zu \> deinstallieren. Deinstallieren Sie [Microsoft Support- und Wiederherstellungs-Assistent,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.

4. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Microsoft 365 Admin Center an, und [installieren Sie Microsoft 365 Apps for Enterprise.](https://portal.office.com/OLS/MySoftware.aspx)

5. Nachdem Office installiert wurde, ***öffnen oder melden Sie sich nicht*** bei Office Anwendungen an.

6. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer, indem Sie die Registrierung wie folgt bearbeiten:

1. Klicken Sie mit der rechten Maustaste auf die Schaltfläche Windows in der unteren linken Ecke des Bildschirms, und wählen Sie "Ausführen" aus. Geben Sie im Feld "Öffnen" **"regedit"** ein, und wählen Sie dann "OK" aus.

2. Wählen Sie "Ja" aus, wenn Sie aufgefordert werden, dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu erlauben.

3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration hinzu.

7. Melden Sie sich auf dem RDS-Server ***als Endbenutzer an,*** und [stellen Sie sicher, dass die Aktivierung freigegebener Computer für Microsoft 365 Apps for Enterprise aktiviert ist.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Weitere Informationen zu den Voraussetzungen, Setupanweisungen und Anleitungen zu angepassten Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Bereitstellen von Microsoft 365 Apps for Enterprise mithilfe von Remotedesktopdiensten.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung freigegebener Computer finden Sie unter Problembehandlung bei der [Aktivierung freigegebener Computer für Microsoft 365 Apps for Enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  