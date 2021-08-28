---
title: Erstellen und Freigeben von Kalendern für öffentliche Ordner in Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: 7ea393011d270fb342d09107f097fcfe685c67833d5a7106bf46b3c7fab0e352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080529"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a>Erstellen und Freigeben von Kalendern für öffentliche Ordner in Exchange Online

Kalender im öffentlichen Ordner können nur über den Outlook-Desktopclient erstellt werden. Führen Sie die folgenden Schritte aus, um Kalender für öffentliche Ordner einzurichten:

1. Stellen Sie sicher, dass die öffentlichen Ordner in Exchange Online bereitgestellt wurden. Weitere Informationen finden Sie unter [Erstellen eines Postfachs für öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox). 

2. Stellen Sie sicher, dass Sie die erforderlichen Zugriffsberechtigungen zum Erstellen des öffentlichen Ordners besitzen. Weitere Informationen finden Sie unter [Berechtigungen für Öffentliche Ordner für Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server). 
  
3. Melden Sie sich beim Outlook-Desktopclient an, und stellen Sie sicher, dass Sie auf Ihre Bereitstellung öffentlicher Ordner zugreifen können.

    Wenn beim Zugriff auf öffentliche Ordner mit dem Outlook-Desktopclient Probleme auftreten, finden Sie entsprechende Informationen unter [Exchange Online-Benutzer können mithilfe von Outlook oder OWA keine Verbindung mit öffentlichen Ordnern herstellen](https://aka.ms/pfcte).

4. Erstellen Sie einen neuen Kalendertyp für öffentliche Ordner.

Der öffentliche Ordner wird standardmäßig für alle anderen Benutzer freigegeben. Der Besitzer des öffentlichen Ordners kann die Berechtigungen im Outlook-Desktopclient ändern. Weitere Informationen finden Sie unter [Berechtigungen für Öffentliche Ordner für Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).

**Hinweis** Kalender für öffentliche Ordner sind für die Verwendung in der Organisation vorgesehen und können nicht im Internet veröffentlicht werden. Verwenden Sie ein freigegebenes Postfach, wenn Sie einen Kalender im Internet veröffentlichen möchten.