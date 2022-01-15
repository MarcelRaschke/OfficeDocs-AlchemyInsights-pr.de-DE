---
title: Zuordnen einer SharePoint Bibliothek zu einem Netzlaufwerk
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 647a1b09c5b9cc751ec64ad72e3dc78743940a25
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61989810"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Zuordnen einer SharePoint Bibliothek zu einem Netzlaufwerk

Anstatt ein Netzlaufwerk zuzuordnen, synchronisieren Sie SharePoint Dateien mit dem neuen OneDrive-Synchronisation-Client, der Dateien bei Bedarf bereitstellt. Greifen Sie auf alle Ihre Dateien auf OneDrive zu, ohne lokalen Speicherplatz zu verwenden. Weitere Informationen finden Sie unter [Synchronisieren SharePoint und Teams von Dateien mit Ihrem Computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) und Speichern von Speicherplatz mit OneDrive Dateien bei Bedarf für [Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

Wenn Sie ein Laufwerk anstatt [den neuen OneDrive-Synchronisation-Client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)zuordnen möchten, stellen Sie sicher, dass Sie die folgenden Schritte ausführen:

- [Problembehandlung bei zugeordneten Netzwerken, die mit SharePoint Online verbunden sind](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**HINWEIS:** Wenn Sie Internet Explorer 10 mit Windows 8 oder Windows 7 verwenden und beim Zuordnen eines Laufwerks nicht **auf** **"Zugriff verweigert"** zugreifen können, beheben Sie dieses Problem, indem Sie diesen [Hotfix](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)installieren.