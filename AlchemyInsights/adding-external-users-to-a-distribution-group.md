---
title: Hinzufügen externer Benutzer zu einer Verteilergruppe
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.openlocfilehash: 090b82b59fdbdcdcdee41e363e27e1b1e7360464
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66313167"
---
# <a name="add-external-users-to-a-distribution-group"></a>Hinzufügen externer Benutzer zu einer Verteilergruppe

Das Hinzufügen eines externen Kontakts zu einer Verteilergruppe (DG) erfolgt in zwei Schritten:
  
1. Erstellen eines E-Mail-Kontakts für den externen Benutzer:
    
    1. Wechseln Sie im Admin Center zur Seite **"**[Benutzerkontakte](https://admin.microsoft.com/adminportal/home#/Contact) > ". 
    
    2. Wählen Sie **"Kontakt hinzufügen"** aus.
    
    3. Geben Sie die Informationen für Ihren Kontakt ein, und wählen Sie **"Hinzufügen"** aus.
    
2. Fügen Sie den E-Mail-Kontakt zu Ihrer GD hinzu:
    
    1. Wechseln Sie im Admin Center zur Seite **Gruppen** > [Gruppen](https://admin.microsoft.com/adminportal/home#/groups). 
    
    2. Suchen Sie die DG, der Sie den externen Benutzer hinzufügen möchten, und wählen Sie ihn aus, um das Bearbeitungsdialogfeld zu öffnen.
    
    3. Wählen Sie auf der Registerkarte **Mitglieder** die Option **Alle anzeigen und Mitglieder verwalten** aus. 
    
    4. Wählen Sie **Mitglieder hinzufügen** aus.
    
    5. Wählen Sie den E-Mail-Kontakt aus, den Sie im vorherigen Schritt erstellt haben, und wählen Sie dann **"Speichern"** aus.
    
Wenn ihre externen Benutzer nach diesen Schritten keine E-Mails an die GD senden oder keine E-Mails von ihr erhalten können, kann es sein, dass die GD so gekennzeichnet ist, dass sie nur E-Mails von internen Benutzern zulässt. Sie können diese Konfiguration überprüfen und anhand der [hier angegebenen](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online) Anweisungen korrigieren.
  
 **Hinweis:** Diese Anweisungen gelten nicht, wenn der Typ Ihrer Gruppe "Microsoft 365-Gruppe" anstelle von "Verteilergruppe" lautet. Wenn dies der Fall ist, können Sie den externen Benutzer direkt aus Outlook zur Gruppe hinzufügen. Ausführliche Informationen zu Microsoft 365-Gruppen Gästen sowie Anweisungen zum Hinzufügen externer Gäste finden Sie in [diesem Artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  