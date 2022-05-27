---
title: Speichern einer Website oder Liste als Vorlage
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: e87e87a38cf520fb6d33f39b7c40eece0112a76f
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65729872"
---
# <a name="save-site-or-list-as-a-template"></a>Speichern einer Website oder Liste als Vorlage

SharePoint-Websitevorlagen sind vorkonfigurierte Definitionen, die einem bestimmten Geschäftszweck dienen. Weitere Informationen finden Sie unter [Verwenden von Vorlagen zum Erstellen verschiedener Arten von SharePoint Websites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Im Folgenden finden Sie einige häufige Probleme/Lösungen im Zusammenhang mit dem Speichern einer Website oder Liste als Vorlage in SharePoint Online.

**Die Schaltfläche "Website-/Listenvorlage speichern" ist nicht verfügbar oder fehlt**. 

- Administratoren müssen benutzerdefinierte Skripts zulassen, um die Vorlagenfeatures zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie [unter Zulassen oder Verhindern von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Der Befehl "Website als Vorlage speichern" wird nicht unterstützt und kann auf Websites, auf denen die SharePoint Server-Veröffentlichungsinfrastruktur verwendet wird, Probleme verursachen.


**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**

- Möglicherweise fehlt der Vorlage ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature in der aktuellen Websitesammlung nicht aktiviert werden kann, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.


- Überprüfen Sie, ob irgendwelche Listen oder Bibliotheken den oberen [Schwellenwert der Listenansicht](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) von 5000 Elementen überschreiten, da hierdurch die Erstellung einer Websitevorlage verhindert werden kann.


- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.


- Es treten Probleme beim Anzeigen von Daten aus einer Liste auf, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter [Mithilfe einer Vorlage generierte Liste zeigt nicht die Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Ausführlichere Informationen zu allgemeinen Problemen und Lösungen finden Sie unter ["Erstellen und Verwenden von Websitevorlagen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)".

