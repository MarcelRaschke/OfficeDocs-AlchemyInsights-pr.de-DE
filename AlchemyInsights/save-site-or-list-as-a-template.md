---
title: Speichern von Websites oder Listen als Vorlage
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 8718c9e80753065666a8d33f05bb85f1a0870472
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63199574"
---
# <a name="save-site-or-list-as-a-template"></a>Speichern von Websites oder Listen als Vorlage

SharePoint-Websitevorlagen sind vorkonfigurierte Definitionen, die einem bestimmten Geschäftszweck dienen. Weitere Informationen finden Sie unter [Verwenden von Vorlagen zum Erstellen verschiedener Arten von SharePoint Websites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Hier sind einige häufige Probleme/Lösungen im Zusammenhang mit dem Speichern einer Website oder Liste als Vorlage in SharePoint Online.

**Schaltfläche "Website-/Listenvorlage speichern" ist nicht verfügbar oder fehlt**. 

- Administratoren müssen benutzerdefinierte Skripts zulassen, um die Vorlagenfeatures zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter [Zulassen oder Verhindern von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Der Befehl "Website als Vorlage speichern" wird nicht unterstützt und kann auf Websites, auf denen die SharePoint Server-Veröffentlichungsinfrastruktur verwendet wird, Probleme verursachen.


**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**

- Möglicherweise fehlt der Vorlage ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature in der aktuellen Websitesammlung nicht aktiviert werden kann, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.


- Überprüfen Sie, ob irgendwelche Listen oder Bibliotheken den oberen [Schwellenwert der Listenansicht](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) von 5000 Elementen überschreiten, da hierdurch die Erstellung einer Websitevorlage verhindert werden kann.


- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MEGABYTE (MB).


- Es treten Probleme beim Anzeigen von Daten aus einer Liste auf, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter "[Durch Vorlagen generierte Liste zeigt keine Daten aus der richtigen Nachschlageliste in SharePoint Online" an](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Ausführlichere Informationen zu allgemeinen Problemen und Lösungen finden Sie unter ["Erstellen und Verwenden von Websitevorlagen"](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

