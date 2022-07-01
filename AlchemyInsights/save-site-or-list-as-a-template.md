---
title: Speichern einer Website oder Liste als Vorlage
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.openlocfilehash: 16742bfe21e3b766a4a95d75a0e3db7170dc3019
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66597119"
---
# <a name="save-site-or-list-as-a-template"></a>Speichern einer Website oder Liste als Vorlage

SharePoint-Websitevorlagen sind vorkonfigurierte Definitionen, die einem bestimmten Geschäftszweck dienen. Weitere Informationen finden [Sie unter Verwenden von Vorlagen zum Erstellen verschiedener Arten von SharePoint-Websites](https://support.microsoft.com/office/create-different-kinds-of-sharepoint-sites-using-site-templates-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Im Folgenden finden Sie einige häufige Probleme/Lösungen im Zusammenhang mit dem Speichern einer Website oder Liste als Vorlage in SharePoint Online.

**Die Schaltfläche "Website-/Listenvorlage speichern" ist nicht verfügbar oder fehlt**. 

- Administratoren müssen benutzerdefinierte Skripts zulassen, um die Vorlagenfeatures zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie [unter Zulassen oder Verhindern von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Der Befehl "Website als Vorlage speichern" wird nicht unterstützt und kann auf Websites, auf denen die SharePoint Server-Veröffentlichungsinfrastruktur verwendet wird, Probleme verursachen.


**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**

- Möglicherweise fehlt der Vorlage ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature in der aktuellen Websitesammlung nicht aktiviert werden kann, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.


- Überprüfen Sie, ob irgendwelche Listen oder Bibliotheken den oberen [Schwellenwert der Listenansicht](https://support.microsoft.com/office/manage-large-lists-and-libraries-b8588dae-9387-48c2-9248-c24122f07c59) von 5000 Elementen überschreiten, da hierdurch die Erstellung einer Websitevorlage verhindert werden kann.


- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.


- Es treten Probleme beim Anzeigen von Daten aus einer Liste auf, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter [Mithilfe einer Vorlage generierte Liste zeigt nicht die Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Ausführlichere Informationen zu allgemeinen Problemen und Lösungen finden Sie unter ["Erstellen und Verwenden von Websitevorlagen](https://support.microsoft.com/office/create-and-use-site-templates-in-sharepoint-server-versions-60371b0f-00e0-4c49-a844-34759ebdd989)".

