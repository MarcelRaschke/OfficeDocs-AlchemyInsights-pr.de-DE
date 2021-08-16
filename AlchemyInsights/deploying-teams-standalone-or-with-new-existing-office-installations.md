---
title: Bereitstellen von Teams als eigenständig oder mit neuen oder vorhandenen Office-Installationen
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102201"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Bereitstellen von Teams als eigenständig oder mit neuen oder vorhandenen Office-Installationen

Microsoft Teams ist jetzt bestandteil von ***Neuinstallationen*** von Microsoft 365 Apps for Enterprise, Microsoft 365 Apps for Business und Office für Mac. Weitere Informationen finden Sie unter ["Wann wird Microsoft Teams in neue Installationen von Office einbezogen?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Darüber hinaus werden ab Version 1906 im aktuellen Kanal Teams ***vorhandenen Installationen*** von Microsoft 365 Apps for Enterprise (und Microsoft 365 Apps for Business) auf Geräten hinzugefügt, die Windows ausgeführt werden, wenn Sie Ihre vorhandene Installation auf die neueste Version aktualisieren. Weitere Informationen finden Sie unter ["Was ist mit vorhandenen Installationen von Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Wenn Sie nicht auf diesen Rollout-Zeitplan warten möchten, können Sie Teams als eigenständig für Ihre Benutzer bereitstellen, indem Sie [diese Anweisungen befolgen,](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) oder Sie können Ihre Benutzer Teams für sich selbst installieren [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) lassen.

Wenn Ihre Organisation nicht bereit ist, Teams bereitzustellen, können Sie Teams von [neuen](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) oder [vorhandenen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Installationen von Office ***ausschließen.*** Wenn sie Teams installieren möchten, aber nicht möchten, dass Teams nach der Installation automatisch für den Benutzer gestartet wird, lesen Sie ["Verhindern, dass Microsoft Teams nach der Installation automatisch gestartet](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)wird.

Informationen zum ***Deinstallieren Teams*** von einem Gerät, auf dem Windows ausgeführt wird, finden Sie unter [Deinstallieren Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Informationen zum Bereinigen Microsoft Teams von mehreren Zielcomputern oder Benutzern finden Sie [unter Microsoft Teams Bereitstellungsbereinigung.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Wenn Sie gemeinsam genutzte Computer, Remotedesktopdienste (RDS) oder virtuelle Desktopinfrastruktur (VDI) verwenden, finden Sie weitere Informationen unter [freigegebene Computer- und VDI-Umgebungen mit Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Wenn Sie Office für Mac verwenden, lesen Sie [Microsoft Teams Installationen auf einem Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Nachdem Teams installiert wurde, wird es ungefähr alle zwei Wochen automatisch mit neuen Features und Qualitätsupdates [aktualisiert.](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 