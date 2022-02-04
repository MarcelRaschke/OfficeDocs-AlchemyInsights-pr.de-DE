---
title: "Fehler bei der Migration öffentlicher Ordner bei 95\_%"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 01/03/2022
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
  - 639
  - 3500007
---

# <a name="public-folder-migration-fails-at-95"></a>Fehler bei der Migration öffentlicher Ordner bei 95 %

Fehler bei Migrationen öffentlicher Ordner bei 95 % mit dem Fehler „FailedToMailEnablePublicFoldersException“:

1. Laden Sie das Skript [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) auf Ihrem lokalen Exchange-Server herunter, und führen Sie es aus.
2. Führen Sie die vom Skript vorgeschlagenen Korrekturmaßnahmen aus.
3. Führen Sie Sync-MailPublicFolders (für Exchange 2010) oder Sync-ModernMailPublicFolders (für Exchange 2013 und höher) aus.
4. Setzen Sie die Migration öffentlicher Ordner fort.
