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
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 164badc302748a70904643f17c68452b5664ef7a
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62753687"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxyadressenfehler beim Erstellen eines Postfachs oder eines anderen E-Mail-aktivierten Objekts

Wenn Sie versucht haben, ein E-Mail-aktiviertes Objekt (Postfach, freigegebenes Postfach usw.) zu erstellen und die Fehlermeldung "Die Proxyadresse "SMTP:alias@domain.com" wird bereits verwendet..." erhalten haben, wird die von Ihnen gewählte E-Mail-Adresse bereits von einem anderen E-Mail-aktivierten Objekt in Ihrer Organisation verwendet.
  
Sie müssen den Benutzer, die Gruppe, das freigegebene Postfach oder den öffentlichen Ordner mit dieser E-Mail-Adresse suchen und löschen oder seine E-Mail-Adresse ändern. Anschließend können Sie ein neues E-Mail-aktiviertes Objekt mit der freigegebenen E-Mail-Adresse erstellen. Verwenden Sie die Suche auf der Startseite, um sie zu finden. Sie können auch den folgenden Exchange Online PowerShell-Befehl verwenden, um nach ihm zu suchen:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Wenn Sie die vorhandene E-Mail-Adresse nicht löschen möchten, wählen Sie eine neue E-Mail-Adresse für das neue Objekt aus, das Sie erstellen.
  