---
title: Installieren von Office und OneDrive auf Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590294"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installieren von Office und OneDrive auf Windows Virtual Desktop

1. [Vorbereiten und Anpassen eines VHD-Masterbilds](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Erstellen Sie einen virtuellen Computer (VM), wenn er noch nicht erstellt wurde.

1. [Installieren Sie Office im Aktivierungsmodus gemeinsam genutzter Computer](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Die Aktivierung gemeinsam genutzter Computer ermöglicht mehreren Benutzern den Zugriff auf Office.

1. [Installieren Sie OneDrive im Computermodus](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalerweise wird OneDrive pro Benutzer installiert, sollte aber hier pro Computer installiert werden.