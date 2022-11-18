---
title: Reagieren auf einen kompromittierten Connector
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010041"
- "17368"
ms.date: 05/19/2022
ms.openlocfilehash: 15578c4d058a525255ee4a520781a2c91201eeec
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66430349"
---
# <a name="respond-to-a-compromised-connector"></a>Reagieren auf einen kompromittierten Connector

Ein kompromittierter eingehender Connector ist, wenn eine nicht autorisierte Person Änderungen entweder auf einen vorhandenen eingehenden Connector anwendet oder einen neuen eingehenden Connector mit der Absicht erstellt, Spam- oder Phishing-E-Mails zu senden. Untersuchen und beheben Sie die kompromittierten Connectors und Konten:

- Überprüfen Sie die sendende IP in der [Warnung "Verdächtige Connectoraktivität"](https://security.microsoft.com/alerts).
- Verwenden Sie die Domäne und IP-Adresse, um Nachrichten im [Exchange Admin Center](https://admin.exchange.microsoft.com/#/messagetrace) oder im Explorer nachzuverfolgen, wenn Sie über eine E5- oder Defender für Office 365 P2-Lizenz verfügen.
- Durchsuchen Sie das Überwachungsprotokoll im [Microsoft Purview Compliance Center](https://compliance.microsoft.com/audit) , um zu ermitteln, wer den verdächtigen Connector erstellt/geändert hat.

Weitere Informationen finden Sie unter:

[Reagieren auf einen kompromittierten Connector](https://docs.microsoft.com/microsoft-365/security/office-365-security/respond-compromised-connector)

[Reagieren auf ein kompromittiertes E-Mail-Konto](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)

[Entfernen blockierter Connectors aus dem Portal für eingeschränkte Entitäten](https://docs.microsoft.com/microsoft-365/security/office-365-security/remove-blocked-connectors)

[Suchen Sie das Überwachungsprotokoll im Microsoft Purview Compliance Portal.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)