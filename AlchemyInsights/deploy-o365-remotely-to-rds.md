---
title: Bereitstellen von Microsoft 365 Apps für die gemeinsame Verwendung auf RDS, Terminalserver oder VDI
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 70f8e725c7bc4006ea1ebac0af6e94f6bec06fb3
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62555895"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Bereitstellen von Microsoft 365 Apps für die gemeinsame Verwendung auf RDS, Terminalserver oder VDI

Um Microsoft 365 Apps mithilfe von Remotedesktopdiensten (RDS), früher Terminaldienste, bereitzustellen, müssen Sie:

- Verwenden Sie den einfachen Fix, um TLS 1.2 standardmäßig zu aktivieren, wenn Sie eine ältere Version von Windows ausführen (z. B. Windows 7 SP1, Windows Server 2008 R2). Eine einfache Lösung und weitere Informationen finden Sie unter [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- Sie verfügen über einen Plan, der Microsoft 365 Apps for Enterprise (zuvor Office 365 Plus) enthält. Beispielsweise Office 365 E3 oder Microsoft 365 E5 oder einen Plan, der die Desktopversion von Project oder Visio enthält, z. B. Project Plan 3 oder Visio Plan 2 oder Microsoft 365 Business Premium Plan, der auch Microsoft 365 Apps for Business umfasst.
- Aktivieren sie die Aktivierung freigegebener Computer. Weitere Informationen finden Sie unter [Übersicht über die Aktivierung freigegebener Computer für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Hinweis**: Um Microsoft 365 Apps im Aktivierungsmodus für gemeinsam genutzte Computer zu installieren, laden Sie die [Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) herunter, und führen Sie sie aus. Ausführliche Informationen zu den Voraussetzungen, Setupanweisungen und Anleitungen zum Anpassen von Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Bereitstellen von Microsoft 365 Apps mithilfe von Remotedesktopdiensten](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter:

- [Problembehandlung bei der Aktivierung freigegebener Computer für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Aktivierungsstatus von Microsoft 365 Apps für Unternehmen zurücksetzen](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Wenn Sie Microsoft 365 Apps auf RDS über das Microsoft 365 Admin Center installieren möchten, das standardinstallationseinstellungen verwendet, führen Sie die folgenden Schritte aus:

1. Überprüfen Sie, über welchen Microsoft 365 Plan Sie verfügen. Weitere Informationen finden Sie unter ["Welches Abonnement habe ich?"](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Wechseln Sie bei Bedarf zu einem anderen Microsoft 365 Plan. Weitere Informationen finden Sie unter [Upgrade auf einen anderen Plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Wenn Microsoft 365 Apps bereits mit anderen inkompatiblen Plänen auf dem RDS-Server installiert ist, deinstallieren Sie sie, indem Sie zu **"Systemsteuerunguninstall** > **" eines Programms wechseln**. Wenn Probleme auftreten, deinstallieren Sie, indem Sie [Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) herunterladen.

1. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Microsoft 365 Admin Center an, und [installieren Sie Office](https://portal.office.com/OLS/MySoftware.aspx).

   Nachdem Office installiert wurde, öffnen oder melden Sie sich nicht bei Office Anwendungen an.

1. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer, indem Sie die Registrierung bearbeiten:

   1. Klicken Sie mit der rechten Maustaste auf die Schaltfläche Windows in der unteren linken Ecke des Bildschirms, und wählen Sie **"Ausführen**" aus. Geben Sie regedit in das Feld **Öffnen** ein, und klicken Sie dann auf **OK**.

   1. Wenn Sie aufgefordert werden, dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu erlauben, wählen Sie **"Ja**" aus.

   1. Fügen Sie im Registrierungs-Editor unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung **1** hinzu.

1. Melden Sie sich auf dem RDS-Server als Endbenutzer an, und stellen Sie sicher, dass die Aktivierung freigegebener Computer für Microsoft 365 Apps aktiviert ist. 

   Ausführliche Informationen finden [Sie unter Überprüfen, ob die Aktivierung freigegebener Computer für Microsoft 365 Apps aktiviert ist](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).