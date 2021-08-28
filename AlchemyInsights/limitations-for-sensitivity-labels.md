---
title: Einschränkungen für Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: 376c0293c325a725c117d54bb0f15b0146b9224c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332816"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Einschränkungen für Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive

Beachten Sie beim Aktivieren von Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive die Anforderungen und Einschränkungen, darunter:

- SharePoint und OneDrive können einige mit Office-Desktop-Apps gekennzeichnete und verschlüsselte Dateien nicht verarbeiten, wenn die Dateien PowerQuery-Daten, von benutzerdefinierten Add-Ins gespeicherte Daten oder benutzerdefinierte XML-Teile enthalten.
- Vertraulichkeitsbezeichnungen werden nicht automatisch von SharePoint und OneDrive auf die vorhandene Dateien angewendet, die Sie bereits mit Azure Information Protection (AIP)-Bezeichnungen verschlüsselt haben. So wenden Sie Vertraulichkeitsbezeichnungen auf verschlüsselte Dateien an: 
    - Stellen Sie sicher, dass AIP-Bezeichnungen migriert und im Microsoft 365 Compliance Center veröffentlicht wurden.
    - Laden Sie die gekennzeichneten Dateien herunter, und laden Sie sie dann an ihren ursprünglichen SharePoint- oder OneDrive-Speicherort hoch.
- Bei verschlüsselten Dokumenten wird das Drucken nicht unterstützt.

Weitere Informationen zu Einschränkungen finden Sie unter [Aktivieren von Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
