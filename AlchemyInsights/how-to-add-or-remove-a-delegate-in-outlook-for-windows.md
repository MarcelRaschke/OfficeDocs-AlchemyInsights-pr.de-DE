---
title: Hinzufügen oder Entfernen eines Delegaten in Outlook für Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 4777e708eac0d425edc852cbf02bcdbd9e2057e7
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62651262"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Hinzufügen oder Entfernen eines Delegaten in Outlook für Windows

So fügen Sie einen Delegaten in Outlook für Windows hinzu: 

1. Klicken Sie auf die Registerkarte **"Datei**", gefolgt von **"Konto Einstellungen**", und wählen Sie dann "**Zugriff delegieren" aus**.
2. Klicken Sie auf **"Hinzufügen"**. Wenn **"Hinzufügen**" nicht angezeigt wird, ist möglicherweise keine aktive Verbindung zwischen Outlook und Exchange vorhanden. Die Outlook Statusleiste zeigt den Verbindungsstatus an.
3. Geben Sie den Namen der Person ein, die Sie als Stellvertretung festlegen möchten, oder suchen Sie, und wählen Sie den Namen in der Liste der Suchergebnisse aus.

    **Hinweis**: Der Delegat muss eine Person in der globalen Adressliste (GAL) Exchange Ihrer Organisation sein.
4. Klicken Sie auf **"Hinzufügen"** , gefolgt von **"OK"**.
5. Akzeptieren Sie im Dialogfeld Berechtigungen **delegieren** die Standardberechtigungseinstellungen, oder wählen Sie benutzerdefinierte Zugriffsebenen für Exchange Ordner aus.

    - Wenn ein Stellvertreter die Berechtigung benötigt, nur mit Besprechungsanfragen und -antworten zu arbeiten, sind die Standardberechtigungseinstellungen, z. B **. Stellvertretung erhält Kopien von Besprechungsnachrichten, die an mich gesendet** werden, ausreichend. Sie können die Einstellung für die **Berechtigung "Posteingang** " bei **"None**" belassen. Besprechungsanfragen und -antworten gehen direkt an den Posteingang der Stellvertretung.

    **Hinweis**: Standardmäßig wird der Stellvertretung die **Berechtigung "Editor" (kann Elemente lesen, erstellen und ändern)** für Ihren **Kalenderordner** gewährt. Wenn die Stellvertretung in Ihrem Namen auf eine Besprechung antwortet, wird sie automatisch ihrem **Kalenderordner** hinzugefügt.

5. Um eine Nachricht zu senden, um den Delegaten über die geänderten Berechtigungen zu benachrichtigen, aktivieren Sie das Kontrollkästchen " **Nachricht automatisch senden, um diese Berechtigungen zu delegieren"** .
6. Wenn Sie möchten, aktivieren Sie das Kontrollkästchen **"Stellvertretung kann meine privaten Elemente sehen** ".

    **Wichtig**: Diese Einstellung wirkt sich auf alle Exchange Ordner aus. Dazu gehören alle Ordner "E-Mail", "Kontakte", "Kalender", "Aufgaben", "Notizen" und "Journal". Es gibt keine Möglichkeit, zugriff auf private Elemente nur in angegebenen Ordnern zu gewähren.

7. Wählen Sie **OK** aus.

    **Hinweis**:
    - Nachrichten, die mit den Berechtigungen "Senden im Auftrag von" gesendet werden, enthalten sowohl die Namen der Stellvertretung als auch Ihre Namen neben **"Von"**. Wenn eine Nachricht mit den Berechtigungen "Senden als" gesendet wird, wird nur Ihr Name angezeigt.
    - Nachdem Sie eine Person als Stellvertretung hinzugefügt haben, kann sie Ihr Exchange Postfach zu ihrem Outlook Profil hinzufügen. Anweisungen finden Sie unter [Verwalten der E-Mail- und Kalenderelemente einer anderen Person](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

So entfernen Sie einen Delegaten in Outlook für Windows:

1. Klicken Sie auf die Registerkarte **"Datei** ".
2. Klicken Sie auf **"Konto Einstellungen** gefolgt von **Delegate Access"**.
3. Wählen Sie den Namen des Delegaten aus, für den Sie Berechtigungen ändern möchten, und klicken Sie dann auf **"Entfernen** ", gefolgt von **"OK"**.
