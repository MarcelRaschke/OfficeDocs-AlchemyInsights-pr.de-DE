---
title: Fehler bei der Migration öffentlicher Ordner bei 95 %
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 01/03/2022
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 9b0ab0e35d6bee1536fb1c237f82bf709b81b4c7
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63126245"
---
# <a name="public-folder-migration-fails-at-95"></a>Fehler bei der Migration öffentlicher Ordner bei 95 %

Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:

1. Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.
2. Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.
3. Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.
4. Setzen Sie die Migration öffentlicher Ordner fort.
