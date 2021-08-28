---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075039"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

In SharePoint und OneDrive beschränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen, indem Sie nur Gruppen oder Einzelpersonen Zugriff gewähren, auf die Sie Zugriff haben möchten. Standardmäßig werden Berechtigungen in SharePoint von höher nach oben in der Hierarchie geerbt. Eine Datei erbt also ihre Berechtigungen vom Ordner, der ihre Berechtigungen von der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.
  
Sie können die Freigabe auf einer höheren Ebene (z. B. durch die Freigabe einer ganzen Website) durchführen und dann die Vererbung unterbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten. Dies wird jedoch nicht empfohlen, da die Verwaltung der Berechtigungen in Zukunft komplexer und verwirrender wird. Sie können stattdessen folgende Aktionen ausführen:
  
- Wenn Sie beispielsweise den gesamten Inhalt eines Ordners mit Ausnahme einer Datei darin freigeben möchten, verschieben Sie diese Datei an einen neuen Speicherort, der nicht freigegeben ist.
    
- Wenn sich zwei Unterordner in einem Ordner befinden und Sie einen Unterordner für die Gruppen A und B freigeben und nur Gruppen-A-Zugriff auf den zweiten Unterordner gewähren möchten, teilen Sie den übergeordneten Ordner mit Gruppe A, und fügen Sie gruppe B zum ersten Unterordner hinzu.
    
[Beenden der Freigabe einer Datei oder eines Ordners ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

