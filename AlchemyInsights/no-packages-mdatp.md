---
title: Keine Pakete MDATP auf RHEL 6.10 verfügbar
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9010721"
- "17402"
ms.date: 06/09/2022
ms.openlocfilehash: b24d41a0a7b77572acbf5c6f23b7be9808bd822c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66308134"
---
# <a name="no-packages-mdatp-available-on-rhel-610"></a>Keine Pakete MDATP auf RHEL 6.10 verfügbar

So installieren Sie MDE auf RHEL 6.10:

1. Verwenden Sie zum Registrieren des Repositorys `sudo yum-config-manager --add-repo=https://packages.microsoft.com/config/rhel/6/prod.repo`.
1. Um die Konfiguration des Repositorys abzurufen, führen Sie `yum -v repolist packages-microsoft-com-prod` aus.
1. Ausführen `yum install`.