---
title: Abrechnung des Kaufs reservierter Instanzen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 639dc40f3be5481c52e4c353fb252ddcb5980387
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63175387"
---
# <a name="billing-for-reserved-instance-purchase"></a>Abrechnung des Kaufs reservierter Instanzen

Der Kauf reservierter Instanzen wird über die Zahlungsmethode abgerechnet, die mit dem Abonnement verknüpft ist, das Sie zum Kaufzeitpunkt auswählen. Bei dem Abonnement muss es sich um ein Enterprise Agreement (Angebotsnummer: MS-AZR-0017P), Pay-As-You-Go (Angebotsnummer: MS-AZR-0003P), eine Microsoft-Kundenvereinbarung oder CSP handeln.

- Bei einem Enterprise-Abonnement werden die Gebühren von dem Saldo der finanziellen Verpflichtung des Abonnements abgezogen, oder als Überschreitung berechnet.
- Bei einem Pay-As-You-Go-Abonnement werden die Gebühren über die Kreditkarte oder Zahlungsmethode des Abonnements abgerechnet.

**Reservierung stornieren**

- **Self-Service:** Sie können eine reservierte Instanz mithilfe von [Azure Portal-](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)selbst stornieren oder austauschen. Wählen Sie die Reservierung aus, und klicken Sie auf zurückerstatten oder austauschen. Bitte beachten Sie, dass Sie auf dem Reservierungsauftrag Inhaberzugriff haben müssen, um austauschen oder zurückerstatten zu können. Wenn Sie nur auf die Reservierung zugreifen, können Sie die Rückerstattung oder den Umtausch nicht fortsetzen. Bitten Sie den Besitzer des Reservierungsauftrags, Ihnen Inhaberzugriff auf den Reservierungsauftrag zu erteilen.
- **Exchange-Richtlinie:** Sie können eine Reservierung für eine andere Reservierung desselben Typs tauschen – es gibt **kein Bußgeld** bei Reservierungsaustausch. Die Gesamtverpflichtung mit neuer Buchung sollte höher sein als die Summe der Erstattungsbeträge der ausgetauschten Reservationen und der künftigen monatlichen Zahlungen (sofern zutreffend).
- **Erstattungsrichtlinie:** Summe der Erstattung und der annullierten künftigen Zahlungen dürfen in einem laufenden 12-monatigen Fenster $50.000 USD nicht überschreiten. Wir **berechnen aktuell kein Bußgeld** für Erstattungen, aber könnten sie für zukünftige Erstattungen berechnen.

**Ausnahmen:** Self-Service-Umtausch- und Stornierungsmöglichkeit sind für Kunden in US-Behörden nicht verfügbar

- **API / PS / CLI** Support steht nicht für Stornierung und Rückerstattungen zur Verfügung [Self-Service-Umtausche und Erstattungen für Azure-Reservierungen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Self-Service Exchange- und Stornierungsmöglichkeit sind für Kunden von US Government Enterprise Agreement nicht verfügbar. Weitere US Government-Abonnementtypen einschließlich Nutzungsbasierte Zahlung und CSP werden unterstützt

Weitere Informationen: [Wie Rückgabe- und Exchange-Transaktionen verarbeitet werden](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Erfahren Sie mehr: [Exchange und Rückerstattungsrichtlinien](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Weitere Fragen: [Besuchen Sie reservierte Instanz-Dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tauschen einer vorhandenen reservierten Instanz (Self-Service)**

Sie können eine Reservierung für eine andere Reservierung desselben Typs tauschen. Sie können auch eine Reservierung von bis zu $50.000 USD pro Jahr erstatten, wenn Sie sie nicht mehr benötigen. Self-Service Exchange- und Stornierungsmöglichkeit sind für Kunden von US Government Enterprise Agreement nicht verfügbar. Weitere US Government-Abonnementtypen einschließlich Nutzungsbasierte Zahlung und CSP werden unterstützt. Sie müssen auf dem Reservierungsauftrag Inhaberzugriff haben, um austauschen oder zurückerstatten zu können.

In den folgenden Schritten wird beschrieben, wie Sie die Transaktion ausführen.

1.Melden Sie sich bei Ihrem [Azure-Portal an](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wählen Sie die Reservierungen aus, die Sie zurückerstatten möchten, und klicken Sie auf **Exchange** 2.Wählen Sie das VM-Produkt aus, das Sie kaufen möchten, und geben Sie eine Menge ein. Stellen Sie sicher, dass die Summe der neuen Einkäufe größer als die Rückgabesumme ist [. Ermitteln Sie vor dem Kauf die richtige Größe](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Überprüfen und Abschließen der Transaktion

**Rückerstattung für eine reservierte Instanz**

Wenn Sie eine Reservierung zurückerstatten möchten, wechseln Sie zu **Reservierungsdetails** und klicken Sie auf **Rückerstattung**

**Anteilige Rückerstattung:**

**Pro-Ration und Mindestanforderungsbeispiele für Erstattung und Vorabreservierung** austauschen:

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

**Rechnung für den letzten Abrechnungszeitraum kann nicht angezeigt werden**

Einige mögliche Gründe, warum möglicherweise keine Rechnung angezeigt wird:

- Sie haben einen monatlichen Kreditbetrag mit Ihrem Abonnement, den Sie nicht überschritten haben, oder Sie haben eine kostenlose Testversion. Eine Rechnung wird nur generiert, wenn Sie Geld abzahlen.
- Es dauert weniger als 30 Tage ab dem Tag, an dem Sie Azure abonniert haben.
- Die Rechnung wird noch nicht generiert. Warten bis zum Ende des Abrechnungszeitraums
- Wenn Sie nicht der Kontoadministrator sind, stehen Ihnen möglicherweise ältere Rechnungen nicht zur Verfügung.

**Herunterladen Ihrer Rechnung aus dem Azure-Portal (.pdf)**

- Wählen Sie Ihr Abonnement auf der Seite ["Abonnements"](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) im Azure-Portal als [Benutzer mit Zugriff auf Rechnungen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support) aus.
- **Auswählen von Rechnungen**
- Klicken Sie auf **Rechnung herunterladen**, um eine Kopie Ihrer PDF-Rechnung anzuzeigen. Wenn **Nicht verfügbar** angezeigt wird, lesen Sie [Warum wird keine Rechnung für den letzten Abrechnungszeitraum angezeigt?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).

**Empfangen Ihrer Rechnung per E-Mail (.pdf)**

- Wählen Sie Ihr Abonnement auf der Seite ["Abonnements"](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) aus. Klicken Sie auf **"Rechnungen"** und dann auf "E-Mail an meine Rechnung senden".
- Klicken Sie auf **"Anmelden"** , und akzeptieren Sie die Bedingungen. Sie müssen sich für jedes Abonnement anmelden, das Sie besitzen.

Hinweis: Wenn Sie nach dem Ausführen der Schritte keine E-Mail erhalten, stellen Sie sicher, dass Ihre E-Mail-Adresse in den [Kommunikationseinstellungen ihres Profils](https://account.windowsazure.com/profile) korrekt ist.

**Herunterladen Ihrer Nutzungsdaten aus dem Azure-Portal**

- Melden Sie sich beim [Azure-Kontocenter](https://account.windowsazure.com/Subscriptions) als [Kontoadministrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) an.
- Wählen Sie das Abonnement aus, für das Sie die Rechnung und nutzungsinformationen benötigen.
- **Auswählen des Abrechnungsverlaufs**
- Wählen Sie **"Aktuelle Anweisung anzeigen" aus** , um eine Schätzung Ihrer Gebühren zum Zeitpunkt der Generierung der Schätzung anzuzeigen.
- Wählen Sie **"Nutzung herunterladen"** aus, um die täglichen Nutzungsdaten als CSV-Datei herunterzuladen. Wenn zwei Versionen verfügbar sind, laden Sie Version 2 herunter.

Weitere Fragen: [reservierte Instanzdokumente besuchen](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Empfohlene Dokumente**

- [Grundlagen der Abrechnung](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verstehen, wie der Rabatt für reservierte Instanzen angewendet wird](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Herunterladen oder Anzeigen Ihrer Azure-Abrechnungsrechnung und der täglichen Nutzungsdaten](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verstehen, wie der Rabatt für reservierte Instanzen angewendet wird](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Grundlegendes zur Verwendung von reservierten Instanzen für Ihr Abonnement für "Pay-As-You-Go"](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Grundlegendes zur Verwendung der reservierten Instanz für Ihre Enterprise-Registrierung](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows Softwarekosten, die nicht in reservierten Instanzen enthalten sind](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reservierte Instanzen im Partner Central Cloud Solution Provider (CSP)-Programm](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)