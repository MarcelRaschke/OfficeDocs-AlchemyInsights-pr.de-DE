---
title: Bereitstellen von Microsoft 365 Apps für die gemeinsame Verwendung auf RDS, Terminal Server oder VDI
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001419"
- "3411"
ms.date: ''
ms.openlocfilehash: 70fbd8ecab2d467117494a819ae928638fd77e25
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66341386"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Bereitstellen von Microsoft 365 Apps für die gemeinsame Verwendung auf RDS, Terminal Server oder VDI

Um Microsoft 365 Apps mithilfe von Remotedesktopdiensten (Remote Desktop Services, RDS), vormals Terminaldienste, bereitzustellen, müssen Sie Folgendes ausführen:

- Verwenden Sie die einfache Lösung, um TLS 1.2 standardmäßig zu aktivieren, wenn Sie eine ältere Version von Windows ausführen (z. B. Windows 7 SP1, Windows Server 2008 R2). Eine einfache Behebung und weitere Informationen finden Sie unter [Update, um TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows zu aktivieren](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- Verfügen Sie über einen Plan, der Microsoft 365 Apps for Enterprise (zuvor Office 365 Plus) enthält. Beispielsweise Office 365 E3 oder Microsoft 365 E5 oder ein Plan, der die Desktopversion von Project oder Visio enthält, z. B. Project Plan 3 oder Visio Plan 2, oder den Microsoft 365 Business Premium-Plan, der auch Microsoft 365 Apps for Business.
- Aktivieren sie die Aktivierung gemeinsam genutzter Computer. Weitere Informationen finden Sie [unter Übersicht über die Aktivierung gemeinsam genutzter Computer für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Hinweis**: Um Microsoft 365 Apps im Aktivierungsmodus für gemeinsam genutzte Computer zu installieren, laden Sie den [Microsoft-Support- und Wiederherstellungs-Assistenten herunter, und führen Sie diesen aus](https://aka.ms/SaRA_OfficeSCA_M365Portal). Ausführliche Informationen zu den Voraussetzungen, Setupanweisungen und Anleitungen zum Anpassen von Installationen mithilfe des Office-Bereitstellungstools finden [Sie unter Bereitstellen von Microsoft 365 Apps mithilfe von Remotedesktopdiensten](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter:

- [Behandlung von Problemen mit der Aktivierung eines gemeinsam genutzten Computers für Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Aktivierungsstatus von Microsoft 365 Apps für Unternehmen zurücksetzen](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Wenn Sie Microsoft 365 Apps auf RDS über die Microsoft 365 Admin Center installieren möchten, die Standardinstallationseinstellungen verwendet, führen Sie die folgenden Schritte aus:

1. Überprüfen Sie, über welchen Microsoft 365-Plan Sie verfügen. Weitere Informationen finden Sie unter [Welches Abonnement habe ich?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Wechseln Sie bei Bedarf zu einem anderen Microsoft 365-Plan. Weitere Informationen finden Sie unter [Zu einem anderen Plan wechseln](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Wenn Microsoft 365 Apps bereits mit anderen inkompatiblen Plänen auf dem RDS-Server installiert ist, deinstallieren Sie es, indem Sie ein Programm **Systemsteuerung** >  **Einstallieren**. Wenn Probleme auftreten, deinstallieren Sie Microsoft-Support [und den Wiederherstellungs-Assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto bei der Microsoft 365 Admin Center an, und [installieren Sie Office](https://portal.office.com/OLS/MySoftware.aspx).

   Nachdem Office installiert wurde, öffnen Sie keine Office-Anwendungen oder melden Sie sich bei diesen an.

1. Aktivieren Sie auf dem RDS-Server die Aktivierung gemeinsam genutzter Computer, indem Sie die Registrierung bearbeiten:

   1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie **"Ausführen**" aus. Geben Sie regedit in das Feld **Öffnen** ein, und klicken Sie dann auf **OK**.

   1. Wenn Sie aufgefordert werden, dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu gestatten, wählen Sie **"Ja**" aus.

   1. Fügen Sie im Registrierungs-Editor unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung **1** hinzu.

1. Melden Sie sich auf dem RDS-Server als Endbenutzer an, und stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Microsoft 365 Apps aktiviert ist. 

   Ausführliche Informationen finden [Sie unter Überprüfen, ob die Aktivierung gemeinsam genutzter Computer für Microsoft 365 Apps aktiviert ist](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).