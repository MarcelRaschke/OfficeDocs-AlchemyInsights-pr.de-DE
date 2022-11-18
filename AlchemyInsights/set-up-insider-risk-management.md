---
title: Microsoft Purview Insider-Risikomanagement einrichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002284"
- "4405"
ms.openlocfilehash: 58a7f6c014673f3236498272ef24196c34f81315
ms.sourcegitcommit: b7ec572b250ab6a4e140e36a64db063df3e55c24
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2022
ms.locfileid: "67070266"
---
# <a name="set-up-microsoft-purview-insider-risk-management"></a>Microsoft Purview Insider-Risikomanagement einrichten

Für den Zugriff auf und die Nutzung des Microsoft Purview Insider-Risikomanagements muss Ihre Organisation über eines der folgenden Abonnements verfügen:

- Microsoft 365 G5-Abonnement (kostenpflichtige oder Testversion)
- Microsoft 365 G3-Abonnement mit dem Microsoft 365 G5-Compliance-Add-On
- Microsoft 365 G3-Abonnement und das Microsoft 365 G5 Insider Risikomanagement-Add-On
- Office 365 E3 Abonnement + Enterprise Mobility and Security E3 + das Microsoft 365 E5 Compliance-Add-On

Wenn Sie keinen vorhandenen Microsoft 365 E5-Plan besitzen und das Microsoft Purview Insider-Risikomanagement testen möchten, können Sie Ihrem vorhandenen Abonnement Microsoft 365 hinzufügen oder sich für eine Testversion von Microsoft 365 Enterprise E5 registrieren.

**Tipps**:

- Stellen Sie mithilfe der Vorlage „Dataleaks“ sicher, dass mindestens eine Microsoft Purview Data Loss Prevention-Richtlinie konfiguriert ist. Es gibt jedoch eine neue Triggeroption, für die keine DLP-Richtlinie konfiguriert werden muss.

- Globale Administratoren haben standardmäßig keinen Zugriff auf das Insider-Risikomanagementportal. Ihnen muss eine der Insider-Risikomanagementrollen zugewiesen werden.

- Wenn einem Administrator keine Warnungen angezeigt werden, stellen Sie sicher, dass der Benutzer einer der folgenden Gruppen zugewiesen ist:

  - Insider-Risikomanagement-Analysten.
  - Insider-Risikomanagement-Prüfer

Weitere Informationen dazu, wie Insider-Risikorichtlinien Ihnen bei der Verwaltung von Risiken in Ihrer Organisation helfen können, finden Sie unter [Informationen zum Insider-Risikomanagement](https://docs.microsoft.com/microsoft-365/compliance/insider-risk-management).