---
title: Für Migrationsbatch für öffentliche Ordner mit CompletedWithErrors-Status
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068163"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Für Migrationsbatch für öffentliche Ordner mit CompletedWithErrors-Status

Führen Sie die folgenden Schritte aus, um den Batch abzuschließen und die großen/ungültigen Elemente zu überspringen: 
1. Genehmigen der übersprungenen Elemente im Migrationsbatch:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Verwenden Sie den folgenden Befehl, um die übersprungenen Elemente für Migrationsanforderungen zu genehmigen, die "Synchronisiert" sind, aber nicht abgeschlossen sind:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Der Migrationsbatch und die Anforderungen sollten innerhalb weniger Minuten fortgesetzt und abgeschlossen werden.

