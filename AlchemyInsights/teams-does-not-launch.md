---
title: Teams kann nicht gestartet werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9007646"
- "12673"
ms.date: 08/4/2021
ms.openlocfilehash: 0bf7df79c749af76b23f7321d3fd5d3a52a55133
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66382557"
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