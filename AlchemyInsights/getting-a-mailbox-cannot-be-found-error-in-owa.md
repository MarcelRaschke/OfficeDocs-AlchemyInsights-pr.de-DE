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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 7c8f35b626ceadc06b830b889bfdf6f2e3e1af74
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63307229"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Fehlermeldung "Postfach nicht gefunden" in Outlook im Web erhalten?

Wenn Sie einen OWA-Fehler (Outlook Web App) erhalten: "Ein Postfach konnte für *den Benutzer* nicht gefunden werden." bedeutet dies, dass der angemeldete Benutzer keine Exchange Onlince-Lizenz und sp hat, dass diesem Benutzerkonto kein Exchange Online Postfach zugeordnet ist. 

Ein Organisationsadministrator kann dem Benutzer über die Microsoft 365 Admin Center eine Exchange Lizenz zuweisen, indem er die folgenden Schritte ausführt:

1. Wechseln Sie zu ["Aktive Benutzer](https://portal.office.com/adminportal/home#/users)", wählen Sie den Benutzer aus, und wählen Sie **"Product LicensesEdit** > **" aus**. 
1. Legen Sie den erforderlichen Speicherort fest.
1. Weisen Sie eine Lizenz zu, die über einen Exchange Online Serviceplan verfügt.