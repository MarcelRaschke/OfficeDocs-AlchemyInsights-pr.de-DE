---
title: Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 7e83dbf916cc2937c853eed10bbbbd48b0680544
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61947959"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>Der Migrationsbatch für öffentlicher Ordner wird nicht abgeschlossen und als synchronisiert angezeigt

Möglicherweise haben Sie den Abschluss des Migrationsbatch eingeleitet, und der Status des Migrationsbatch zeigt noch sehr lange "Synchronisiert" an. Dies ist ein erwartetes Verhalten.

Es ist üblich, dass der Migrationsbatchstatus einige Stunden lang auf Synchronisiert stehen bleibt, bevor er zu Wird abgeschlossen wechselt. Bei Migrationen mit einer großen Anzahl von Zielpostfächern ist es normal, dass der Status Synchronisiert länger als 24 Stunden zu sehen ist, sofern keine der zugrunde liegenden Migrationsanforderungen für öffentliche Ordner fehlgeschlagen ist oder isoliert wurde. Bitte warten Sie 24 - 48 Stunden, bis der Migrationsbatch die Aufgaben abgeschlossen hat.
