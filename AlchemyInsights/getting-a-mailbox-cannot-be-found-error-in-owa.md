---
title: 126 Fehler beim Abrufen eines Postfachs in OWA nicht gefunden?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: f0dc80992fbbd64d5812560b8372bb2f2391a4fe
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62685355"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Fehlermeldung "Postfach nicht gefunden" in Outlook im Web erhalten?

Wenn Sie einen OWA-Fehler (Outlook Web App) erhalten: "Ein Postfach konnte für *den Benutzer* nicht gefunden werden." bedeutet dies, dass der angemeldete Benutzer nicht über eine Exchange Onlince-Lizenz und sp verfügt, kein Exchange Online Postfach diesem Benutzerkonto zugeordnet ist. 

Ein Organisationsadministrator kann dem Benutzer über die Microsoft 365 Admin Center eine Exchange Lizenz zuweisen, indem er die folgenden Schritte ausführt:

1. Wechseln Sie zu ["Aktive Benutzer](https://portal.office.com/adminportal/home#/users)", wählen Sie den Benutzer aus, und wählen Sie **"Product LicensesEdit** > **" aus**. 
1. Legen Sie den erforderlichen Speicherort fest.
1. Weisen Sie eine Lizenz zu, die über einen Exchange Online Serviceplan verfügt.