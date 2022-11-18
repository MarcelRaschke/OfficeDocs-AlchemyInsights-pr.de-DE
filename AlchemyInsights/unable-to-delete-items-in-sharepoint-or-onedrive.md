---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000255"
- "1851"
- "2377"
ms.openlocfilehash: 5ff74a867623d6ecff8d9ea1b86f4b63b8dea0f3
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66600217"
---
# <a name="unable-to-delete-items"></a>Elemente können nicht gelöscht werden.

- Aufbewahrungsrichtlinien können dies verursachen. Sie müssen entweder den jeweiligen Haltebereich deaktivieren oder ausschließen, der dieses Problem verursacht. Nachdem eine Aufbewahrungsrichtlinie oder ein Haltebereich entfernt wurde, kann es bis zu 24 Stunden dauern, bis die Änderung wirksam wird. Stellen Sie sicher, dass für das Element keine [Aufbewahrungsrichtlinie](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) eingerichtet ist.

- Möglicherweise hat die Website den Speichergrenzwert überschritten, das [Websitekontingent](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps&preserve-view=true) erhöht und das Element gelöscht.

- Stellen Sie sicher, dass das Element nicht für einen anderen Benutzer [ausgecheckt](https://support.microsoft.com/office/check-out-check-in-or-discard-changes-to-files-in-a-sharepoint-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.

- Schließlich können Administratoren [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation&preserve-view=true) (PnP) verwenden, das eine Bibliothek von PowerShell-Befehlen enthält, mit denen Sie komplexe Verwaltungsaktionen ausführen können, z. B. das Löschen hartnäckiger Elemente.
- [PNP-Datei entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPFile.md)
- [PNP-Ordner entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPFolder.md)
- [PNP-Listenelement entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPListItem.md)
- [PNP-Liste entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPList.md)
- [PNP-Feld entfernen (Spalte)](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPField.md)
