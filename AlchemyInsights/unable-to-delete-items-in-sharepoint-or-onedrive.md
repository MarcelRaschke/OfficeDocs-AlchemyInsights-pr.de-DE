---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038516"
---
# <a name="unable-to-delete-items"></a>Elemente können nicht gelöscht werden

- Aufbewahrungsrichtlinien können dies verursachen. Sie müssen entweder die entsprechende Aufbewahrung deaktivieren oder ausschließen, die dieses Problem verursacht. Nachdem eine Aufbewahrungsrichtlinie oder aufbewahrungssperre entfernt wurde, kann es bis zu 24 Stunden dauern, bis die Änderung wirksam wird. Stellen Sie sicher, dass für das Element keine [Aufbewahrungsrichtlinie](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) eingerichtet ist.

- Die Website hat möglicherweise das Speicherlimit überschritten, das [Websitekontingent](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) erhöht und das Element gelöscht.

- Stellen Sie sicher, dass das Element nicht für einen anderen Benutzer [ausgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.

- Schließlich können Administratoren [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) verwenden, die eine Bibliothek von PowerShell-Befehlen enthält, mit denen Sie komplexe Verwaltungsaktionen ausführen können, z. B. das Erzwingen des Löschens von Stub stiftelementen.
- [Entfernen der PNP-Datei](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Entfernen des PNP-Ordners](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Entfernen eines PNP-Listenelements](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Entfernen der PNP-Liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Entfernen des PNP-Felds (Spalte)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)