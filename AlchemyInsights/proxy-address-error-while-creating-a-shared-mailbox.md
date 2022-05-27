---
title: Proxyadressenfehler beim Erstellen eines freigegebenen Postfachs
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: a60fdd860a7a7a542cc33094b9128c2274b08c66
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65728611"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxyadressenfehler beim Erstellen eines Postfachs oder eines anderen E-Mail-aktivierten Objekts

Wenn Sie versucht haben, ein E-Mail-fähiges Objekt (Postfach, freigegebenes Postfach usw.) zu erstellen und die Fehlermeldung "Die Proxyadresse "SMTP:alias@domain.com" wird bereits verwendet..." erhalten haben, wird die von Ihnen ausgewählte E-Mail-Adresse bereits von einem anderen E-Mail-aktivierten Objekt in Ihrer Organisation übernommen.
  
Sie müssen den Benutzer, die Gruppe, das freigegebene Postfach oder den öffentlichen Ordner mit dieser E-Mail-Adresse suchen und löschen oder seine E-Mail-Adresse ändern. Anschließend können Sie ein neues E-Mail-aktiviertes Objekt mit der freigegebenen E-Mail-Adresse erstellen. Verwenden Sie die Suche auf der Startseite, um sie zu finden. Sie können auch den folgenden Exchange Online PowerShell-Befehl verwenden, um danach zu suchen:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Wenn Sie die vorhandene E-Mail-Adresse nicht löschen möchten, wählen Sie eine neue E-Mail-Adresse für das neue Objekt aus, das Sie erstellen.
  