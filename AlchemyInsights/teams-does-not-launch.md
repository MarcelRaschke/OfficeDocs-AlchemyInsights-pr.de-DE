---
title: Teams kann nicht gestartet werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: b178db48f81731fe78dc0ee406c4d71cb887647f
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63189896"
---
# <a name="teams-doesnt-launch"></a>Teams kann nicht gestartet werden

Wenn Sie versuchen, Microsoft Teams zu öffnen, aber es startet nie, versuchen Sie Folgendes:

1. Browsen Sie zu **%appdata%\Microsoft\Teams**.
1. Löschen Sie den Inhalt des Ordners.
1. Starten Sie den Computer neu, und versuchen Sie, Teams zu starten.

Möglicherweise müssen Sie Teams erneut installieren. Um es erneut zu installieren:

1. Deinstallieren Sie Teams über die Systemsteuerung.
1. Browsen Sie zu **%appdata%\Microsoft\Teams\Application Cache**.
1. Löschen Sie den Inhalt des Ordners.
1. Browsen Sie zu **%appdata%\Microsoft\teams\Cache**.
1. Löschen Sie den Inhalt des Ordners.
1. Starten Sie den Computer neu, und laden Sie dann Teams herunter und installieren Sie es.

Wenn Sie in Ihrem Mandanten eine Diagnose für einen bestimmten Benutzer, der sich nicht anmelden kann, durchführen möchten, starten Sie eine neue Suche mit dem Schlüsselwort **TeamsUserUnableToSignIn** und folgen Sie den Aufforderungen.