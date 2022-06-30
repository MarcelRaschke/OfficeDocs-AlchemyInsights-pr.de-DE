---
title: Erstellen einer Website in SharePoint Online
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.openlocfilehash: 591b01ab9fd7f22974c99396d25358b7245aa4c0
ms.sourcegitcommit: 8324c868c664bfdee6d5bb99ad8d41e9dd46d10f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66540314"
---
# <a name="create-sharepoint-sites-using-templates"></a>Erstellen von SharePoint-Websites mithilfe von Vorlagen

Die Möglichkeit, eine Website als Vorlage zu speichern, wird von modernen Kommunikations- oder Teamwebsites nicht unterstützt. Weitere Informationen zur Verwendung von Vorlagen finden Sie unter [Speichern, Herunter- und Hochladen einer SharePoint-Website als Vorlage](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Im Folgenden finden Sie einige häufige Probleme/Lösungen im Zusammenhang mit dem Speichern einer Website oder Liste als Vorlage in SharePoint Online. 

**Schaltfläche 'Website-/Listenvorlagen speichern' ist nicht verfügbar oder fehlt**

Administratoren müssen benutzerdefinierte Skripts zulassen, um die Vorlagenfeatures zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter 

- [Zulassen oder Blockieren von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Der Befehl "Website als Vorlage speichern" wird nicht unterstützt und kann auf Websites, auf denen die SharePoint Server-Veröffentlichungsinfrastruktur verwendet wird, Probleme verursachen.

**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**

Möglicherweise fehlt der Vorlage ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature in der aktuellen Websitesammlung nicht aktiviert werden kann, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.

- Überprüfen Sie, ob irgendwelche Listen oder Bibliotheken den oberen [Schwellenwert der Listenansicht](https://support.microsoft.com/office/manage-large-lists-and-libraries-b8588dae-9387-48c2-9248-c24122f07c59) von 5000 Elementen überschreiten, da hierdurch die Erstellung einer Websitevorlage verhindert werden kann.

- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.


- Es treten Probleme beim Anzeigen von Daten aus einer Liste auf, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter [Mithilfe einer Vorlage generierte Liste zeigt nicht die Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Ausführlichere Informationen zu allgemeinen Problemen und Lösungen finden Sie unter [Erstellen und Verwenden von Websitevorlagen](https://support.microsoft.com/office/create-and-use-site-templates-in-sharepoint-server-versions-60371b0f-00e0-4c49-a844-34759ebdd989).



