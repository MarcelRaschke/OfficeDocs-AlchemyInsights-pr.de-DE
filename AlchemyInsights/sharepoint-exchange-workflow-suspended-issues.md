---
title: Erste Schritte mit SharePoint Online
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 32e53dfa157043d70004d949f2648c4af750afb3
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63293009"
---
# <a name="workflows-in-sharepoint"></a>Workflows in SharePoint

Wenn SharePoint Workflows keine E-Mails senden, hat Ihre Organisation möglicherweise die Grenzwerte für Exchange Online Absender erreicht.

Die Fehlermeldung "Workflow ist angehalten" kann auftreten, wenn Sie eines der folgenden Elemente haben:

- Sie verfügen über einen Workflow in SharePoint Online, der den Workflowplattformtyp SharePoint 2010 oder SharePoint 2013 verwendet.

- Der Workflow ist so konfiguriert, dass eine benutzerdefinierte E-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute gesendet wird.

Wenn Sie den Workflow ausführen, wird die E-Mail-Nachricht nicht gesendet, und Sie bemerken die Fehlermeldung, der interne Status ist auf "Angehalten" festgelegt oder kann nicht an einen Empfänger gesendet werden.

Weitere Informationen finden Sie im folgenden [Artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

