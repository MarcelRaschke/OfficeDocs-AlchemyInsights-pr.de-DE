---
title: Reservierung stornieren
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 33f523a51001a1a989adf127a1c2d0d111a6e848
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61947022"
---
# <a name="cancelling-reservation"></a>Reservierung stornieren

- **Self-Service:** Sie können eine reservierte Instanz mithilfe von [Azure Portal-](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)selbst stornieren oder austauschen. Wählen Sie die Reservierung aus, und klicken Sie auf zurückerstatten oder austauschen. Bitte beachten Sie, dass Sie auf dem Reservierungsauftrag Inhaberzugriff haben müssen, um austauschen oder zurückerstatten zu können. Wenn Sie nur auf die Reservierung zugreifen, können Sie die Rückerstattung oder den Umtausch nicht fortsetzen. Bitten Sie den Besitzer des Reservierungsauftrags, Ihnen Inhaberzugriff auf den Reservierungsauftrag zu erteilen.
- **Exchange-Richtlinie:** Sie können eine Reservierung für eine andere Reservierung desselben Typs tauschen – es gibt **kein Bußgeld** bei Reservierungsaustausch. Die Gesamtverpflichtung mit neuer Buchung sollte höher sein als die Summe der Erstattungsbeträge der ausgetauschten Reservationen und der künftigen monatlichen Zahlungen (sofern zutreffend).
- **Erstattungsrichtlinie:** Summe der Erstattung und der annullierten künftigen Zahlungen dürfen in einem laufenden 12-monatigen Fenster $50.000 USD nicht überschreiten. Wir **berechnen aktuell kein Bußgeld** für Erstattungen, aber könnten sie für zukünftige Erstattungen berechnen.  
    **Ausnahmen:** Self-Service-Umtausch- und Stornierungsmöglichkeit sind für Kunden in US-Behörden nicht verfügbar
- **API / PS / CLI** Support steht nicht für Stornierung und Rückerstattungen zur Verfügung [Self-Service-Umtausche und Erstattungen für Azure-Reservierungen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Self-Service Exchange- und Stornierungsmöglichkeit sind für Kunden von US Government Enterprise Agreement nicht verfügbar. Weitere US Government-Abonnementtypen einschließlich Nutzungsbasierte Zahlung und CSP werden unterstützt

Weitere Informationen: [, wie Retourenbuchungen und Exchange-Transaktionen bearbeitet werden](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Weitere Informationen: [Exchange-und Rückerstattungsrichtlinien](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Weitere Fragen: [reservierte Instanzdokumente besuchen](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tauschen einer vorhandenen reservierten Instanz (Self-Service)**

Sie können eine Reservierung für eine andere Reservierung desselben Typs tauschen. Sie können auch eine Reservierung von bis zu $50.000 USD pro Jahr erstatten, wenn Sie sie nicht mehr benötigen. Self-Service Exchange- und Stornierungsmöglichkeit sind für Kunden von US Government Enterprise Agreement nicht verfügbar. Weitere US Government-Abonnementtypen einschließlich Nutzungsbasierte Zahlung und CSP werden unterstützt. Sie müssen auf dem Reservierungsauftrag Inhaberzugriff haben, um austauschen oder zurückerstatten zu können.

In den folgenden Schritten wird beschrieben, wie Sie die Transaktion ausführen.

1. Melden Sie sich bei Ihrem [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)an. Wählen Sie die Reservierungen aus, die Sie zurückerstatten möchten, und klicken Sie auf **Exchange**
2. Wählen Sie das VM-Produkt aus, das Sie kaufen möchten, und geben Sie eine Menge ein. Stellen Sie sicher, dass der neue Gesamtbetrag mehr als der Gesamtbetrag der Rückerstattung ist [Bestimmen Sie die richtige Größe, bevor Sie den Kauf abschließen.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Überprüfen und durchführen der Transaktion

**Rückerstattung für eine reservierte Instanz**

Wenn Sie eine Reservierung zurückerstatten möchten, wechseln Sie zu **Reservierungsdetails** und klicken Sie auf **Rückerstattung**

**Anteilige Rückerstattung:**

**Anteilige und minimale Anforderungsbeispiele für Erstattung und Umtausch**  
Beispiel für die Vorabreservierung:

- Sie kaufen einen RI-Jahreszeitraum für $120 am 1. Januar.
- Am 7. April möchten Sie diese Reservierung zurückerstatten oder austauschen.
- Da die Reservierung seit 97 Tagen erfolgt, erhalten Sie (1-97/365) * $120 zurück. (d. h. $88,1). Derzeit gibt es kein Bußgeld für Erstattungen
- Bei einem Umtausch sollte Ihr neuer Kauf größer als $88,1 sein
- Es gibt kein Bußgeld für Rückerstattung zur Zeit

**Beispiel für einen Abrechnungsplan:**

- Sie kaufen einen RI-Jahreszeitraum für $10 pro Monat
- Am 7. April möchten Sie diese Reservierung zurückerstatten oder austauschen.
- Seit der letzten Zahlung 7 Tage, erhalten Sie (1-7/31) * $10 zurück. (d. h. $7,74).
- Die zukünftig stornierten Zahlungen sind $80. Derzeit gibt es kein Bußgeld für Erstattungen
- Bei dieser Kündigung wird $87,74 von Ihrem $50.000-Erstattungslimit abgezogen.
- Bei einem Umtausch sollte Ihr neuer Kauf größer als $87,74 sein

**Empfohlene Dokumente**

- [Wie Retourenbuchungen und Umtauschtransaktionen bearbeitet werden](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Umtausch- und Rückerstattungsrichtlinien](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)