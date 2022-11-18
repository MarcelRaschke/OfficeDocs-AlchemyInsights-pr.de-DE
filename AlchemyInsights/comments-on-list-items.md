---
title: Kommentare zu Listenelementen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: f5a4404b0af31a0de92c778e3af989f7b24d21dd
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66394887"
---
# <a name="comments-on-list-items"></a>Kommentare zu Listenelementen

Benutzer können alle Kommentare für ein Listenelement anzeigen und zwischen Ansichten filtern, in denen Kommentare oder Aktivitäten im Zusammenhang mit einem Element angezeigt werden.

Benutzer müssen Folgendes beachten, bevor sie Kommentare hinzufügen und löschen können:

- Kommentare folgen den Berechtigungseinstellungen, die SharePoint innewohnen.
- Klassische Listen, die noch nicht so erstellt wurden, dass sie in modernen Benutzeroberflächen angezeigt werden, z. B. Aufgabenlisten, verfügen nicht über dieses Kommentarfeature.
- Das Kommentieren von Listen in Teams ist in dieser Version nicht verfügbar.
- Kommentare werden von der Suche nicht indiziert.

Administratoren können dieses Feature auf Organisationsebene deaktivieren, indem sie den Parameter **CommentsOnListItemsDisabled** im **PowerShell-Cmdlet "Set-SPOTenant** " ändern.

Es ist derzeit nicht möglich, die Kommentarerstellung auf Website- oder Listenebene zu deaktivieren. Wir hoffen, diese Steuerelemente in einem späteren Update zu haben, wahrscheinlich im ersten Quartal 2021.
