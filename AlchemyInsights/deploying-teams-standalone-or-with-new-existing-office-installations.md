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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 9521f892501460dfc134ae63eedddb940cfd2764
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63216035"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Bereitstellen von Teams als eigenständig oder mit neuen oder vorhandenen Office-Installationen

Microsoft Teams ist jetzt bestandteil von ***Neuinstallationen*** von Microsoft 365 Apps for Enterprise, Microsoft 365 Apps for Business und Office für Mac. Weitere Informationen finden Sie unter ["Wann wird Microsoft Teams in neue Installationen von Office aufgenommen?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Darüber hinaus wird Teams ab Version 1906 im aktuellen Kanal ***vorhandenen Installationen*** von Microsoft 365 Apps for Enterprise (und Microsoft 365 Apps for Business) auf Geräten mit Windows hinzugefügt, wenn Sie Ihre vorhandene Installation auf die neueste Version aktualisieren. Weitere Informationen finden Sie unter ["Was ist mit vorhandenen Installationen von Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Hinweis**: Wenn Sie nicht auf diesen Rollout-Zeitplan warten möchten, können Sie Teams als eigenständige Bereitstellung für Ihre Benutzer bereitstellen, indem Sie [diese Anweisungen befolgen](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) , oder Sie können Ihre Benutzer Dazu führen, dass Ihre Benutzer Teams für sich selbst [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)installieren.

Wenn Ihre Organisation nicht bereit ist, Teams bereitzustellen, haben wir die Schritte, die Sie ausführen können, um Teams von [neuen](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) oder [vorhandenen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Installationen von Office ***auszuschließen***. Wenn Sie möchten, dass Microsoft Teams installiert wird, Teams aber nicht automatisch für den Benutzer nach der Installation gestartet wird, lesen Sie " [Verhindern, dass Microsoft Teams nach der Installation automatisch gestartet](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) wird".

Informationen zum ***Deinstallieren von Teams*** von einem Gerät unter Windows finden Sie unter ["Deinstallieren von Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)". Informationen zum Bereinigen von Microsoft Teams von mehreren Zielcomputern oder Benutzern finden Sie unter [Microsoft Teams-Bereitstellungsbereinigung](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Wenn Sie gemeinsam genutzte Computer, Remotedesktopdienste (RDS) oder virtuelle Desktopinfrastruktur (Virtual Desktop Infrastructure, VDI) verwenden, lesen Sie ["Freigegebene Computer- und VDI-Umgebungen mit Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)".

Wenn Sie Office für Mac verwenden, sehen Sie sich [microsoft Teams-Installationen auf einem Mac an](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Hinweis**: Nachdem Teams installiert wurde, wird es ungefähr alle zwei Wochen automatisch mit neuen Features und Qualitätsupdates [aktualisiert](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) . 