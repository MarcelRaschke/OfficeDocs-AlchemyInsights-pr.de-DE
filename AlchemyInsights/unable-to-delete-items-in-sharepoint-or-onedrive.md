---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 9ae841d837d3c6da01909183fba6e8510e36a248
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65593516"
---
# <a name="unable-to-delete-items"></a>Elemente können nicht gelöscht werden.

- Aufbewahrungsrichtlinien können dies verursachen. Sie müssen entweder den jeweiligen Haltebereich deaktivieren oder ausschließen, der dieses Problem verursacht. Nachdem eine Aufbewahrungsrichtlinie oder ein Haltebereich entfernt wurde, kann es bis zu 24 Stunden dauern, bis die Änderung wirksam wird. Stellen Sie sicher, dass für das Element keine [Aufbewahrungsrichtlinie](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) eingerichtet ist.

- Möglicherweise hat die Website den Speichergrenzwert überschritten, das [Websitekontingent](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps&preserve-view=true) erhöht und das Element gelöscht.

- Stellen Sie sicher, dass das Element nicht für einen anderen Benutzer [ausgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.

- Schließlich können Administratoren [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation&preserve-view=true) (PnP) verwenden, das eine Bibliothek mit PowerShell-Befehlen enthält, mit denen Sie komplexe Verwaltungsaktionen ausführen können, z. B. das Löschen hartnäckiger Elemente.
- [PNP-Datei entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPFile.md)
- [PNP-Ordner entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPFolder.md)
- [PNP-Listenelement entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPListItem.md)
- [PNP-Liste entfernen](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPList.md)
- [PNP-Feld entfernen (Spalte)](https://github.com/pnp/powershell/blob/dev/documentation/Remove-PnPField.md)
