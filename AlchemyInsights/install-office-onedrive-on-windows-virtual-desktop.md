---
title: Installieren von Office und OneDrive auf Windows Virtual Desktop
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: bcac970daa39225b2b5f285dd0ba5e9b7ed68d86
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61960737"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installieren von Office und OneDrive auf Windows Virtual Desktop

1. [Vorbereiten und Anpassen eines VHD-Masterbilds](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Erstellen Sie einen virtuellen Computer (VM), wenn er noch nicht erstellt wurde.

1. [Installieren Sie Office im Aktivierungsmodus gemeinsam genutzter Computer](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Die Aktivierung gemeinsam genutzter Computer ermöglicht mehreren Benutzern den Zugriff auf Office.

1. [Installieren Sie OneDrive im Computermodus](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalerweise wird OneDrive pro Benutzer installiert, sollte aber hier pro Computer installiert werden.