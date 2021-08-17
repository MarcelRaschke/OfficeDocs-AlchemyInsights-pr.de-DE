---
title: Erstellen einer Website in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057965"
---
# <a name="create-sharepoint-sites-using-templates"></a>Erstellen SharePoint Websites mithilfe von Vorlagen

Die Möglichkeit, eine Website als Vorlage zu speichern, wird von modernen Kommunikations- oder Teamwebsites nicht unterstützt. Weitere Informationen zur Verwendung von Vorlagen finden Sie unter [Speichern, Herunter- und Hochladen einer SharePoint-Website als Vorlage](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Hier sind einige häufige Probleme/Lösungen im Zusammenhang mit dem Speichern einer Website oder Liste als Vorlage in Sharepoint Online. 

**Schaltfläche "Website-/Listenvorlage speichern" ist nicht verfügbar oder fehlt**

Administratoren müssen benutzerdefinierte Skripts zulassen, um die Vorlagenfeatures zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter 

- [Zulassen oder Blockieren von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Der Befehl "Website als Vorlage speichern" wird nicht unterstützt und kann auf Websites, auf denen die SharePoint Server-Veröffentlichungsinfrastruktur verwendet wird, Probleme verursachen.

**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**

Möglicherweise fehlt der Vorlage ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature in der aktuellen Websitesammlung nicht aktiviert werden kann, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.

- Überprüfen Sie, ob irgendwelche Listen oder Bibliotheken den oberen [Schwellenwert der Listenansicht](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) von 5000 Elementen überschreiten, da hierdurch die Erstellung einer Websitevorlage verhindert werden kann.

- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.


- Es treten Probleme beim Anzeigen von Daten aus einer Liste auf, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter [Mithilfe einer Vorlage generierte Liste zeigt nicht die Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Ausführlichere Informationen zu allgemeinen Problemen und Lösungen finden Sie unter [Erstellen und Verwenden von Websitevorlagen.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



