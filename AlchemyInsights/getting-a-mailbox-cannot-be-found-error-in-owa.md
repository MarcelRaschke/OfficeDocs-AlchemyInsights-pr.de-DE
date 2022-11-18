---
title: 126 Fehler beim Abrufen eines Postfachs in OWA nicht gefunden?
ms.author: chrisda
author: chrisda
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1600020"
- "126"
ms.date: 04/21/2020
ms.openlocfilehash: 909460b16115dce76236d1a4a97c2de45a40d972
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66269128"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Fehlermeldung "Postfach nicht gefunden" in Outlook im Web erhalten?

Wenn eine Outlook Web App (OWA)-Fehlermeldung angezeigt wird: "Ein Postfach konnte für *den Benutzer* nicht gefunden werden". Dies bedeutet, dass der angemeldete Benutzer nicht über eine Exchange Onlince-Lizenz und sp verfügt, kein Exchange Online Postfach diesem Benutzerkonto zugeordnet ist. 

Ein Organisationsadministrator kann dem Benutzer über die Microsoft 365 Admin Center eine Exchange-Lizenz zuweisen, indem er die folgenden Schritte ausführt:

1. Wechseln Sie zu ["Aktive Benutzer](https://admin.microsoft.com/AdminPortal/Home?ref=users)", wählen Sie den Benutzer aus, und wählen Sie " **Produktlizenzen** > **bearbeiten"** aus. 
1. Legen Sie den erforderlichen Speicherort fest.
1. Weisen Sie eine Lizenz zu, die über einen Exchange Online Serviceplan verfügt.