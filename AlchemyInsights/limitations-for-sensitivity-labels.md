---
title: Einschränkungen für Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 31d06305f4fa36629db7295e3eeaa48b885a5326
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62755271"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Einschränkungen für Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive

Beachten Sie beim Aktivieren von Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive die Anforderungen und Einschränkungen, darunter:

- SharePoint und OneDrive können einige mit Office-Desktop-Apps gekennzeichnete und verschlüsselte Dateien nicht verarbeiten, wenn die Dateien PowerQuery-Daten, von benutzerdefinierten Add-Ins gespeicherte Daten oder benutzerdefinierte XML-Teile enthalten.
- Vertraulichkeitsbezeichnungen werden nicht automatisch von SharePoint und OneDrive auf die vorhandene Dateien angewendet, die Sie bereits mit Azure Information Protection (AIP)-Bezeichnungen verschlüsselt haben. So wenden Sie Vertraulichkeitsbezeichnungen auf verschlüsselte Dateien an: 
    - Stellen Sie sicher, dass AIP-Bezeichnungen migriert und im Microsoft 365 Compliance Center veröffentlicht wurden.
    - Laden Sie die gekennzeichneten Dateien herunter, und laden Sie sie dann an ihren ursprünglichen SharePoint- oder OneDrive-Speicherort hoch.
- Bei verschlüsselten Dokumenten wird das Drucken nicht unterstützt.

Weitere Informationen zu Einschränkungen finden Sie unter [Aktivieren von Vertraulichkeitsbezeichnungen für Office-Dateien in SharePoint und OneDrive](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
