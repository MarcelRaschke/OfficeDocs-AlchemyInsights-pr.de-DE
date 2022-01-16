---
title: Wiederherstellen eines gelöschten Formulars
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 61dd6b12049673a811e1636c2f850fa8b7eb6f09
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61982003"
---
# <a name="restore-a-deleted-form"></a>Wiederherstellen eines gelöschten Formulars

Wenn Sie ein Formular versehentlich in Microsoft Forms gelöscht haben, können Sie es wiederherstellen. Melden Sie sich bei Microsoft Forms als Besitzer des gelöschten Formulars an. Wählen Sie den **Papierkorb aus,** wählen Sie dann das Formular aus, das Sie wiederherstellen möchten, und wählen Sie **Wiederherstellen** aus. Wählen Sie nach der Wiederherstellung den Pfeil auf der **Seite "Zurück zu meinen Formularen"** aus.

Nur der Besitzer des Formulars kann es wiederherstellen. Wenn das Konto des Formularbesitzers deaktiviert oder aus dem Mandanten entfernt wurde, kann das Formular nur vom globalen Administrator wiederhergestellt werden. Der globale Administrator muss über eine Forms-Lizenz verfügen, um eine Wiederherstellung ausführen zu können. Nur Formulare, die innerhalb von 30 Tagen erstellt wurden, nachdem das Benutzerkonto deaktiviert oder aus dem Mandanten entfernt wurde, können wiederhergestellt werden.

Wenn Sie der globale Administrator des Mandanten sind und ein Formular aus einem Konto wiederherstellen möchten, das gelöscht oder deaktiviert wurde, ersetzen Sie [E-Mail-Adresse] durch die E-Mail-Adresse des gelöschten oder deaktivierten Benutzers in der folgenden URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner= [E-Mail-Adresse]** Wenn Ihre E-Mail-Adresse beispielsweise johndoe@contoso.com ist, lautet die URL wie folgt: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** . 

Sobald Sie Zugriff auf die gelöschten Formulare des Benutzers haben, wählen Sie das Formular aus, das Sie verschieben möchten, und wählen Sie dann **weitere Formularaktionen**  >  **verschieben** aus.

Wenn Sie ein Formular wiederherstellen möchten, in dem es gelöscht wurde und der Benutzer aus der Organisation entfernt wurde, kann ein globaler Administrator den Benutzer wiederherstellen, das Kennwort für diesen Benutzer zurücksetzen und dann während der Anmeldung als dieser Benutzer auf das Formular zugreifen, um es zu einem anderen aktiven Benutzer zu verschieben. 