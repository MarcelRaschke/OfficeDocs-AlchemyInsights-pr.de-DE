---
title: Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3500007"
- "639"
ms.date: 08/25/2020
ms.openlocfilehash: 51ce400c34dc6422e3fe4a9986c266005e60204d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66292582"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt

Möglicherweise haben Sie den Abschluss eines Migrationsbatches eingeleitet, und der Status des Migrationsbatches wird noch sehr lange als "Synchronisiert" angezeigt. Dieses Verhalten ist zu erwarten.

Es ist üblich, dass der Migrationsbatchstatus einige Stunden lang auf Synchronisiert stehen bleibt, bevor er zu Wird abgeschlossen wechselt. Bei Migrationen mit einer großen Anzahl von Zielpostfächern ist es normal, dass der Status Synchronisiert länger als 24 Stunden zu sehen ist, sofern keine der zugrunde liegenden Migrationsanforderungen für öffentliche Ordner fehlgeschlagen ist oder isoliert wurde. Bitte warten Sie 24 - 48 Stunden, bis der Migrationsbatch die Aufgaben abgeschlossen hat.
