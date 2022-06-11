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
- "17402"
- "9010721"
ms.date: 06/09/2022
ms.openlocfilehash: 73ca261836ff708c1b671faab380e7821a7ea61b
ms.sourcegitcommit: 5121d86fdd8582da70b4bdca88674c0d1ab2b22b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "65998254"
---
# <a name="no-packages-mdatp-available-on-rhel-610"></a>Keine Pakete MDATP auf RHEL 6.10 verfügbar

So installieren Sie MDE auf RHEL 6.10:

1. Verwenden Sie zum Registrieren des Repositorys `sudo yum-config-manager --add-repo=https://packages.microsoft.com/config/rhel/6/prod.repo`.
1. Um die Konfiguration des Repositorys abzurufen, führen Sie `yum -v repolist packages-microsoft-com-prod` aus.
1. Ausführen `yum install`.