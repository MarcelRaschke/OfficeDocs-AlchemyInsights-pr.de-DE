---
title: Erste Schritte mit SharePoint Online
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.openlocfilehash: 176cd191afeb397dfd36afe204aaad408ec0401a
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66384033"
---
# <a name="workflows-in-sharepoint"></a>Workflows in SharePoint

Wenn SharePoint-Workflows keine E-Mails senden, sind in Ihrer Organisation möglicherweise die Grenzwerte für Exchange Online Absender aufgetreten.

Die Fehlermeldung "Workflow ist angehalten" kann auftreten, wenn Sie über eines der folgenden Elemente verfügen:

- Sie haben einen Workflow in SharePoint Online, der den SharePoint 2010- oder SharePoint 2013-Workflowplattformtyp verwendet.

- Der Workflow ist so konfiguriert, dass eine benutzerdefinierte E-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute gesendet wird.

Wenn Sie den Workflow ausführen, wird die E-Mail-Nachricht nicht gesendet, und Sie sehen, dass die Fehlermeldung "Interner Status" auf "Angehalten" festgelegt ist oder "Senden an einen Empfänger nicht möglich" angezeigt wird.

Weitere Informationen finden Sie im folgenden [Artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

