---
title: Fehler bei der Migration öffentlicher Ordner bei 95 %
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 01/03/2022
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 140800f768b716aa12ced0eb2752df83bf88ff8d
ms.sourcegitcommit: 4f75eddd6f210a8d821bedf78dd8b674220c4da3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/04/2022
ms.locfileid: "61710936"
---
# <a name="public-folder-migration-fails-at-95"></a>Fehler bei der Migration öffentlicher Ordner bei 95 %

Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:

1. Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.
2. Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.
3. Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.
4. Setzen Sie die Migration öffentlicher Ordner fort.
