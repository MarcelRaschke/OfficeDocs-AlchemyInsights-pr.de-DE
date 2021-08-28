---
title: Bereitstellen von Microsoft 365 Apps for Enterprise für die gemeinsame Verwendung auf RDS, Terminalserver oder VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325602"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Bereitstellen von Microsoft 365 Apps for Enterprise für die gemeinsame Verwendung auf RDS, Terminalserver oder VDI

So stellen Sie Microsoft 365 Apps for Enterprise mithilfe von Remotedesktopdiensten (RDS) bereit, die früher als Terminaldienste bezeichnet wurden:

- Sie benötigen einen Microsoft 365 For Business-Plan oder einen Office 365-Plan, der Microsoft 365 Apps for Enterprise umfasst, z. B. Office 365 Enterprise E3 oder Enterprise E5.
   **Hinweis:** Die Pläne Microsoft 365 Apps for Business und Microsoft 365 Business Standard enthalten keine Microsoft 365 Apps for Enterprise.
- Sie müssen die [Aktivierung freigegebener Computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)aktivieren.

**Hinweis:** Sie können die [Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) auch herunterladen und ausführen, um Microsoft 365 Apps for Enterprise im Aktivierungsmodus für gemeinsam genutzte Computer zu installieren.

Weitere Informationen zu voraussetzungen, Setup-Anweisungen und Anleitungen für angepasste Installationen mithilfe des Office Bereitstellungstool finden Sie unter [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

So beheben Sie Fehler im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer:

- Informationen zur Problembehandlung bei der [Aktivierung freigegebener Computer finden Sie unter Microsoft 365 Apps for Enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Siehe [Aktivierungsstatus von Microsoft 365 Apps für Unternehmen zurücksetzen](https://go.microsoft.com/fwlink/?linkid=2109218).

Wenn Sie Microsoft 365 Apps for Enterprise auf RDS über die Microsoft 365 Admin Center installieren möchten, ***die standardinstallationseinstellungen verwendet,*** führen Sie die folgenden Schritte aus:

1. Überprüfen Sie, über welches Abonnement Sie verfügen. [Anleitung](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Wechseln Sie bei Bedarf zu einem anderen Abonnement. [Anleitung](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Wenn Office bereits mit anderen Microsoft-Abonnements auf dem RDS-Server installiert ist, deinstallieren Sie es. Wenn Sie beispielsweise zur **Systemsteuerung** wechseln,  >  **deinstallieren Sie ein Programm.** Deinstallieren Sie [Microsoft Support- und Wiederherstellungs-Assistent,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.
4. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Microsoft 365 Admin Center an, und [installieren Sie Microsoft 365 Apps for Enterprise.](https://portal.office.com/OLS/MySoftware.aspx)
5. Nachdem Office installiert wurde, ***öffnen oder melden Sie sich nicht*** bei Office Anwendungen an.
6. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer, indem Sie die Registrierung wie folgt bearbeiten:
   1. Klicken Sie mit der rechten Maustaste auf die Schaltfläche Windows in der unteren linken Ecke des Bildschirms, und wählen Sie **"Ausführen"** aus. Geben Sie regedit in das Feld **Öffnen** ein, und klicken Sie dann auf **OK**.
   2. Wählen Sie **"Ja"** aus, wenn Sie aufgefordert werden, dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu erlauben.
   3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration hinzu.
   4. Melden Sie sich auf dem RDS-Server ***als Endbenutzer an,*** und [stellen Sie sicher, dass die Aktivierung freigegebener Computer für Microsoft 365 Apps for Enterprise aktiviert ist.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
