---
title: Für Migrationsbatch für öffentliche Ordner mit CompletedWithErrors-Status
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 3a0e8257cbecb14722d3e271bd935c3e6a64c239
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63226149"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Für Migrationsbatch für öffentliche Ordner mit CompletedWithErrors-Status

Führen Sie die folgenden Schritte aus, um den Batch abzuschließen und die großen/ungültigen Elemente zu überspringen: 
1. Genehmigen der übersprungenen Elemente im Migrationsbatch:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Verwenden Sie den folgenden Befehl, um die übersprungenen Elemente für Migrationsanforderungen zu genehmigen, die "Synchronisiert" sind, aber nicht abgeschlossen sind:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Der Migrationsbatch und die Anforderungen sollten innerhalb weniger Minuten fortgesetzt und abgeschlossen werden.

