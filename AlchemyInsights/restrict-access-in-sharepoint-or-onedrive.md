---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 9f5397d1004889de6ab55d4524cb8b557322a709
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66291700"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

In SharePoint und OneDrive schränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen ein, indem Sie nur Gruppen oder Personen Zugriff gewähren, auf die Sie zugreifen möchten. Standardmäßig werden Berechtigungen in SharePoint von oben in der Hierarchie geerbt. Eine Datei erbt also ihre Berechtigungen von dem Ordner, der seine Berechtigungen von der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.
  
Sie können die Freigabe auf einer höheren Ebene (z. B. durch Freigeben einer gesamten Website) und dann die Vererbung unterbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten. Dies wird jedoch nicht empfohlen, da die Verwaltung der Berechtigungen in Zukunft komplexer und verwirrender wird. Hier ist, was Sie stattdessen tun könnten:
  
- Wenn Sie z. B. den gesamten Inhalt eines Ordners mit Ausnahme einer Datei darin freigeben möchten, verschieben Sie die Datei an einen neuen Speicherort, der nicht freigegeben ist.
    
- Wenn sie zwei Unterordner in einem Ordner haben und einen Unterordner für die Gruppen A und B freigeben und nur gruppe A zugriff auf den zweiten Unterordner zulassen möchten, geben Sie den übergeordneten Ordner für Gruppe A frei, und fügen Sie gruppe B zum ersten Unterordner hinzu.
    
[Beenden der Freigabe einer Datei oder eines Ordners ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

