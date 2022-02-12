---
title: Aktivieren der Kostenverwaltung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 9bc4c28028745b244c2f5d8f7885fc19f82fd735
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62653206"
---
# <a name="enable-cost-management"></a>Aktivieren der Kostenverwaltung

**Was bedeutet "Kosten sind für Ihre Organisation deaktiviert"?**

Organisationen, die Enterprise Agreement (EA) oder Microsoft Customer Agreement (MCA)-Konten verwenden, können den Zugriff auf Kosteninformationen und Preisinformationen deaktivieren.

Nach der Anmeldung beim Azure-Portal können sie die Abrechnungs-APIs verwenden, um Rechnungen (einmal angemeldet) und Nutzungsdetails programmgesteuert abzurufen.

**So erlauben Sie zusätzlichen Benutzern den Zugriff auf Rechnungen**

1. Wechseln Sie zum **Blatt "Abonnements"** im Azure-Portal.
2. Wählen Sie **"Rechnungen"** und dann **"Zugriff auf Rechnungen" aus**.
3. Aktivieren Sie den Zugriff, und speichern Sie dann die Änderungen, um Benutzern in Abonnementrollen das Herunterladen von Rechnungen zu ermöglichen.

**Hinweis**: Der Kontoadministrator kann auch konfigurieren, dass Rechnungen per E-Mail gesendet werden. Weitere Informationen finden Sie unter [Abrufen Ihrer Rechnung per E-Mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Vorgehensweise Hinzufügen von Benutzern zur Rolle "Abrechnungsleser"**

1. Wechseln Sie zum **Blatt "Abonnements"** im Azure-Portal.
2. Wählen Sie **die Zugriffssteuerung (IAM)** aus, und klicken Sie dann auf **"Hinzufügen**".
3. Wählen Sie auf der Seite "**Rolle auswählen**" den **Abrechnungsleser** aus.
4. Geben Sie die E-Mail des Benutzers ein, den Sie einladen möchten, und klicken Sie dann auf **"OK** ", um die Einladung zu senden.
5. Folgen Sie den Anweisungen in der Einladungs-E-Mail, sich als Abrechnungsleser anzumelden. Weitere Informationen finden Sie unter [Gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Empfohlene Dokumente**

- [Aktivieren von DA- und AO-Ansichten über das EA-Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kosten, die in der Kostenverwaltung enthalten sind](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Unterstützte Microsoft Azure Angebote](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Überprüfen der Kosten in der Kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Bereitstellen des Zugriffs auf Abrechnungsinformationen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Überprüfen des Zugriffs auf eine Microsoft-Kundenvereinbarung](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






