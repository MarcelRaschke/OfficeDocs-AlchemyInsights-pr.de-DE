---
title: Nach dem Upgrade auf macOS 11.6 Big Sur kann kein Konto hinzugefügt werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: df17851f6f5e6dd2b18befe5b2582cf18e54e7f2
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63270305"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Nach dem Upgrade auf macOS 11.6 Big Sur kann kein Konto hinzugefügt werden

Nach dem Upgrade auf macOS 11.6 wird Ihr OneDrive für Geschäfts-, Schul- oder Ihr persönliches Konto möglicherweise nicht in Ihrer Kontenliste angezeigt, und Sie können sich möglicherweise nicht bei einem zweiten Konto in der App anmelden.

Für dieses Problem wurde ein Fix entwickelt. Ermitteln Sie zunächst, ob Sie die eigenständige Version oder die App-Store-Version von OneDrive ausführen:

- Wählen Sie die OneDrive Cloud in der Menüleiste > **Hilfe und Einstellungen** > **Einstellungen** > **Info**. Wenn die Versionsnummer nicht enthalten ist **(Eigenständig)**,verfügen Sie über die App Store Version des Produkts.

Wenn Sie die eigenständige Version von OneDrive verwenden, starten Sie Ihren Computer neu, und OneDrive aktualisiert automatisch auf einen Build, bei dem dieses Problem behoben ist. Wenn Sie den Build manuell installieren möchten, laden Sie diese [.zip Datei](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)herunter, entzippen Sie die Datei, und kopieren Sie die OneDrive App in den „Anwendungen“-Ordner (indem Sie die vorhandene OneDrive-App ersetzen).

Wenn Sie die App Store-Version verwenden, sollten Sie erwägen, die eigenständige Version von OneDrive zu installieren. Diese Version funktioniert auf die gleiche Weise wie die App Store-Version, ermöglicht es Microsoft jedoch, Benutzern Updates schneller anzubieten und sie mit einer Version zu verbinden, die die Behebung dieses Problems enthält.

1. Laden Sie die eigenständige Version von [OneDrive herunter, die den Fix enthält.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Entzippen Sie die Datei, und kopieren Sie die OneDrive App in den „Anwendungen“-Ordner (indem Sie die vorhandene OneDrive-App ersetzen).

Wenn Sie die App Store-Version verwenden müssen, warten Sie, bis eine App-Store-Version der App veröffentlicht wird, die die Korrektur enthält. Leider kann Microsoft kein geschätztes Datum für die Veröffentlichung einer festen Version aus dem App Store mitteilen.


