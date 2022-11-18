---
title: Für Migrationsbatch für öffentliche Ordner mit CompletedWithErrors-Status
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 556d930dfd30c27fc64c178ed34d177572681265
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66269200"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Für Migrationsbatch für öffentliche Ordner mit CompletedWithErrors-Status

Führen Sie die folgenden Schritte aus, um den Batch abzuschließen und die großen/fehlerhaften Elemente zu überspringen: 
1. Genehmigen sie die übersprungenen Elemente im Migrationsbatch:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Verwenden Sie den folgenden Befehl, um die übersprungenen Elemente für Migrationsanforderungen zu genehmigen, die "synchronisiert", aber nicht abgeschlossen sind:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Der Migrationsbatch und die Anforderungen sollten in wenigen Minuten fortgesetzt und abgeschlossen werden.

