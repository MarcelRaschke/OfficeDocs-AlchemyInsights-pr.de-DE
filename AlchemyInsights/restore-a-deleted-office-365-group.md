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
ms.openlocfilehash: 9af1b95170e3514625d6658c41df39332084f3d4
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65735204"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Wiederherstellen einer gelöschten Microsoft 365-Gruppe

Sie können eine gelöschte Microsoft 365 Gruppe oder Microsoft Teams innerhalb von 30 Tagen nach dem Löschvorgang wiederherstellen.

1. Wechseln Sie zum [Microsoft 365 Admin Center](https://aka.ms/RestoreDeletedGroup), um sich bei einer Liste der gelöschten Gruppen und Teams anzumelden.

    **Hinweis:** Melden Sie sich mit dem Konto an, das entweder dem Mandantenadministrator oder der Administratorrolle "Gruppen" zugewiesen ist.

1. Wählen Sie die gelöschte Microsoft 365 Gruppe/Teams aus, die wiederhergestellt werden soll, und klicken Sie auf **"Gruppe wiederherstellen"**.

    Wenn die Gruppe aufgrund einer in Konflikt stehenden SMTP-Adresse nicht wiederhergestellt werden kann, verwenden Sie den folgenden Befehl, um das Objekt zu finden, das den Konflikt verursacht, und entfernen Sie die SMTP-Adresse:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Hinweis:** In einigen Fällen kann es bis zu 24 Stunden dauern, bis die Gruppe und alle ihre Daten wiederhergestellt wurden.

    Weitere Informationen oder informationen zum Wiederherstellen von Gruppen mithilfe von PowerShell finden Sie unter [Wiederherstellen einer gelöschten Microsoft 365 Gruppe](https://go.microsoft.com/fwlink/?linkid=867802).