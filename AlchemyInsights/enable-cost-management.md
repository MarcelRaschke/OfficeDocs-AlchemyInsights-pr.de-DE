---
title: Aktivieren des Kostenmanagements
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003547"
- "6463"
ms.date: 12/03/2020
ms.openlocfilehash: 02232c0d21e29270f94e208217c3d7a0259acfac
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66378399"
---
# <a name="enable-cost-management"></a>Aktivieren des Kostenmanagements

**Was bedeutet "Kosten sind für Ihre Organisation deaktiviert"?**

Organisationen, die Enterprise Agreement(EA)- oder Microsoft-Kundenvereinbarung(MCA)-Konten verwenden, können den Zugriff auf Kosteninformationen und Preisinformationen deaktivieren.

Nach der Anmeldung bei Azure-Portal können sie die Abrechnungs-APIs verwenden, um Rechnungen (nach der Anmeldung) und Nutzungsdetails programmgesteuert abzurufen.

**So ermöglichen Sie weiteren Benutzern den Zugriff auf Rechnungen**

1. Wechseln Sie zum **Blatt "Abonnements"** in Azure-Portal.
2. Wählen Sie **"Rechnungen** " und dann **"Zugriff auf Rechnungen" aus**.
3. Aktivieren Sie den Zugriff, gefolgt vom Speichern der Änderungen, um Benutzern in Rollen mit Abonnementbereich das Herunterladen von Rechnungen zu ermöglichen.

**Hinweis**: Der Kontoadministrator kann auch konfigurieren, dass Rechnungen per E-Mail gesendet werden. Weitere Informationen finden Sie unter ["Abrufen Ihrer Rechnung per E-Mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)".

**Hinzufügen von Benutzern zur Rolle "Abrechnungsleser"**

1. Wechseln Sie zum **Blatt "Abonnements"** in Azure-Portal.
2. Wählen Sie **das Zugriffssteuerelement (Access Control, IAM)** aus, und klicken Sie dann auf **"Hinzufügen"**.
3. Wählen Sie " **Abrechnungsleser** " auf der Seite **"Rolle auswählen"** aus.
4. Geben Sie die E-Mail des Benutzers ein, den Sie einladen möchten, und klicken Sie dann auf **"OK** ", um die Einladung zu senden.
5. Folgen Sie den Anweisungen in der Einladungs-E-Mail, um sich als Rechnungsleser anzumelden. Weitere Informationen finden Sie unter [Gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Empfohlene Dokumente**

- [Aktivieren von DA- und AO-Ansichten über das EA-Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kosten, die im Kostenmanagement enthalten sind](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Unterstützte Microsoft Azure-Angebote](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Kosten in der Kostenanalyse überprüfen](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Bereitstellen des Zugriffs auf Abrechnungsinformationen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Überprüfen des Zugriffs auf eine Microsoft-Kundenvereinbarung](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






