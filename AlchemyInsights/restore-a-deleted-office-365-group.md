---
title: Wiederherstellen einer gelöschten Microsoft 365-Gruppe
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 1d9707e9a27aa2c3b57e16acaec5e4d51b4a026a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63222549"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Wiederherstellen einer gelöschten Microsoft 365-Gruppe

Sie können eine gelöschte Microsoft 365 Gruppe oder Microsoft Teams innerhalb von 30 Tagen nach dem Löschen wiederherstellen.

1. Wechseln Sie zu den [Microsoft 365 Admin Center](https://aka.ms/RestoreDeletedGroup), um sich bei einer Liste der gelöschten Gruppen und Teams anzumelden.

    **Hinweis:** Melden Sie sich mit dem Konto an, das entweder dem Mandantenadministrator oder der Gruppenadministratorrolle zugewiesen ist.

1. Wählen Sie die gelöschte Microsoft 365 Gruppe/Teams aus, die wiederhergestellt werden soll, und klicken Sie auf **"Gruppe wiederherstellen"**.

    Wenn die Gruppe aufgrund einer widersprüchlichen SMTP-Adresse nicht wiederhergestellt werden kann, verwenden Sie den folgenden Befehl, um das Objekt zu suchen, das einen Konflikt verursacht, und entfernen Sie die SMTP-Adresse:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Hinweis:** In einigen Fällen kann es bis zu 24 Stunden dauern, bis die Gruppe und alle ihre Daten wiederhergestellt wurden.

    Weitere Informationen oder Informationen zum Wiederherstellen von Gruppen mithilfe von PowerShell finden Sie unter ["Wiederherstellen einer gelöschten Microsoft 365 Gruppe"](https://go.microsoft.com/fwlink/?linkid=867802).