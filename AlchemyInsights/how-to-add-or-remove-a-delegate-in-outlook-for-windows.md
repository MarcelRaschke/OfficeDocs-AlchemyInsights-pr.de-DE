---
title: Hinzufügen oder Entfernen einer Stellvertretung in Outlook für Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 201910ba5b02ad3892dff55aaecaa7ab6177c6e7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66406732"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Hinzufügen oder Entfernen einer Stellvertretung in Outlook für Windows

So fügen Sie eine Stellvertretung in Outlook für Windows hinzu: 

1. Klicken Sie auf die Registerkarte **"Datei** " gefolgt von **"Kontoeinstellungen"**, und wählen Sie dann " **Stellvertretungszugriff**" aus.
2. Klicken Sie auf **"Hinzufügen"**. Wenn **"Hinzufügen"** nicht angezeigt wird, ist möglicherweise keine aktive Verbindung zwischen Outlook und Exchange vorhanden. In der Outlook-Statusleiste wird der Verbindungsstatus angezeigt.
3. Geben Sie den Namen der Person ein, die Sie als Stellvertretung festlegen möchten, oder suchen Sie, und wählen Sie den Namen in der Liste der Suchergebnisse aus.

    **Hinweis**: Bei der Stellvertretung muss es sich um eine Person in der globalen Exchange-Adressliste (GAL) Ihrer Organisation handeln.
4. Klicken Sie auf **"Hinzufügen"** , gefolgt von **"OK"**.
5. Akzeptieren Sie im Dialogfeld " **Berechtigungen delegieren** " die Standardberechtigungseinstellungen, oder wählen Sie benutzerdefinierte Zugriffsebenen für Exchange-Ordner aus.

    - Wenn eine Stellvertretung die Berechtigung benötigt, nur mit Besprechungsanfragen und -antworten zu arbeiten, reichen die **Standardberechtigungseinstellungen wie "Stellvertretung" aus, die Kopien von Besprechungsnachrichten empfängt, die an mich gesendet** wurden. Sie können die Berechtigungseinstellung " **Posteingang** " bei **"Keine**" belassen. Besprechungsanfragen und -antworten gehen direkt in den Posteingang der Stellvertretung.

    **Hinweis**: Standardmäßig wird der Stellvertretung die Berechtigung **"Editor" (kann Elemente lesen, erstellen und ändern)** für Ihren **Kalenderordner** erteilt. Wenn die Stellvertretung in Ihrem Auftrag auf eine Besprechung antwortet, wird sie automatisch ihrem **Kalenderordner** hinzugefügt.

5. Wenn Sie eine Nachricht senden möchten, um den Stellvertreter über die geänderten Berechtigungen zu benachrichtigen, aktivieren Sie das Kontrollkästchen **"Nachricht automatisch an Stellvertretung senden** ", in dem diese Berechtigungen zusammengefasst werden.
6. Aktivieren Sie bei Bedarf das Kontrollkästchen **"Stellvertretung kann meine privaten Elemente anzeigen** ".

    **Wichtig**: Diese Einstellung wirkt sich auf alle Exchange-Ordner aus. Dazu gehören alle Ordner "E-Mail", "Kontakte", "Kalender", "Aufgaben", "Notizen" und "Journal". Es gibt keine Möglichkeit, nur in angegebenen Ordnern Zugriff auf private Elemente zu gewähren.

7. Wählen Sie **OK** aus.

    **Hinweis**:
    - Nachrichten, die mit den Berechtigungen "Im Auftrag senden" gesendet werden, enthalten sowohl die Namen der Stellvertretung als auch Ihre Namen neben **"Von**". Wenn eine Nachricht mit den Berechtigungen "Senden als" gesendet wird, wird nur Ihr Name angezeigt.
    - Nachdem Sie eine Person als Stellvertretung hinzugefügt haben, kann sie Ihr Exchange-Postfach zu ihrem Outlook-Profil hinzufügen. Anweisungen hierzu finden [Sie unter Verwalten der E-Mail- und Kalenderelemente einer anderen Person](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

So entfernen Sie eine Stellvertretung in Outlook für Windows:

1. Klicken Sie auf die Registerkarte **"Datei** ".
2. Klicken Sie auf **"Kontoeinstellungen"** , gefolgt von **"Stellvertretungszugriff**".
3. Wählen Sie den Namen der Stellvertretung aus, für die Sie Berechtigungen ändern möchten, und klicken Sie dann auf **"Entfernen"** , gefolgt von **"OK"**.
