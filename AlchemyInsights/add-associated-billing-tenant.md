---
title: Hinzufügen eines zugeordneten Abrechnungsmandanten
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
ms.reviewer: amberb, vikdesai
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- commerce_billing
- "9011175"
- "17960"
ms.date: 08/17/2022
ms.openlocfilehash: 1be4beb91cacafa1c5ee39196b22dbac65a4b8ac
ms.sourcegitcommit: b52a81c62e8ec915617cf4939abf271139b87f69
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2022
ms.locfileid: "67408569"
---
# <a name="add-an-associated-billing-tenant"></a>Hinzufügen eines zugeordneten Abrechnungsmandanten

Sie müssen ein Abrechnungskontobesitzer sein, um eine Abrechnungsbeziehung mit mehreren Mandanten einzurichten, und sie müssen entweder die Mandanten-ID oder den primären Domänennamen für den Mandanten haben, den Sie einladen möchten. Weitere Informationen finden Sie unter ["Grundlegendes zu Abrechnungskonten](https://docs.microsoft.com/microsoft-365/commerce/manage-billing-accounts) " und ["Suchen einer Mandanten-ID oder eines Domänennamens"](https://aka.ms/findtenantiddomain).

1. Wechseln Sie im Admin Center zur Seite "**Abrechnungskonten** > ".
2. Wählen Sie den Namen des Abrechnungskontos aus, das Sie als primären Abrechnungsmandanten verwenden möchten.
3. Wählen Sie auf der Seite "Abrechnungskontodetails" die Registerkarte **"Zugeordnete Abrechnungsmandanten** " und dann " **Zugeordneten Abrechnungsmandanten hinzufügen"** aus.
4. **Geben Sie im Bereich "Zugeordneten Abrechnungsmandanten hinzufügen**" die Mandanten-ID oder den Domänennamen ein, und geben Sie dann einen Anzeigenamen für den Mandanten ein.
5. Wählen Sie im Abschnitt **"Access-Einstellungen"** eine oder beide Optionen für **die Bereitstellung** und **Abrechnungsverwaltung** aus.
6. Lesen Sie das Kontrollkästchen neben der Sichtbarkeitsanweisung des Benutzers, und wählen Sie es aus.
7. Wählen Sie **"Mandanten hinzufügen"** aus.

Wenn die Einstellung für den **Bereitstellungszugriff** aktiviert ist, wird ein eindeutiger Link erstellt, den Sie an den globalen Administrator des zugeordneten Abrechnungsmandanten senden können. Sie müssen die Bereitstellungsanforderung akzeptieren, bevor Sie Abonnements in ihren Mandanten verschieben können. Weitere Informationen finden [Sie unter "Abrechnung über mehrere Mandanten hinweg verwalten" in der Microsoft 365 Admin Center](https://docs.microsoft.com/microsoft-365/commerce/billing-and-payments/manage-multi-tenant-billing).
