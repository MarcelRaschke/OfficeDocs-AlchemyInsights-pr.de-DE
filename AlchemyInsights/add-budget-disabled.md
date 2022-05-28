---
title: Warum ist die Schaltfläche "Budget hinzufügen" für mich deaktiviert?
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
- "9003547"
- "6464"
ms.openlocfilehash: 7c63eee7583c4210d3d0ed7f2eb39397e95fa355
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65722748"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Warum ist die Schaltfläche "Budget hinzufügen" für mich deaktiviert?

Zum Erstellen eines Budgets benötigen Sie eine der folgenden Berechtigungen:

- Verwaltungsgruppe, Abonnement, Ressourcengruppenbereiche
- Mitwirkender im Kostenmanagement
- Besitzer
- Contributor
- nur Enterprise Kunden: Registrierung, Abteilung, Kontobereiche
- Registrierung Admin (Budget im Registrierungsbereich festlegen)
- Abteilung Admin (Budget auf Abteilungsebene festlegen)
- Kontobesitzer (Budget auf Kontobereich festlegen)
- Nur moderne Kundenvereinbarung: Abrechnungskonto, Abrechnungsprofil, Rechnungsabschnittsbereiche
- Ersteller des Azure-Abonnements

**Ich habe ein Budget erstellt, als meine Kosten für den aktuellen Monat bereits über dem Budget lagen. Warum habe ich keine Benachrichtigung erhalten?**  
Wenn Sie beim Erstellen eines Budgets bereits einen bestimmten Kostenschwellenwert überschritten haben, wird diese Warnung nicht ausgelöst. Sobald ein neuer Zyklus beginnt, wird die Warnung ausgelöst, wenn Sie den Schwellenwert überschreiten.

**Wann sollte ich erwarten, eine Benachrichtigung zu erhalten, nachdem ich einen meiner definierten Schwellenwerte für die Budgetwarnung überschritten habe?**  
Budgets werden alle 4 Stunden ausgewertet. Es dauert mindestens 8 Stunden, bis Nutzungsdaten das Budgetsystem erreicht haben. In diesem Fall kann es bis zu 12 Stunden dauern, bis Warnungen ausgelöst werden, nachdem Sie einen Schwellenwert überschritten haben.

**Warum ist die Schaltfläche "Startdatum" deaktiviert, wenn ich einen Zurücksetzungszeitraum für den Monat oder den Abrechnungsmonat auswähle?**  
Die Budgets werden an den aktuellen Kalendermonat oder den aktuellen Abrechnungszeitraum angepasst (in dem Fall, in dem der Abrechnungsmonat ausgewählt ist). Daher füllen wir diesen Wert vorab für Sie aus.

**Warum sehe ich in der Budgeterstellungsoberfläche kein Diagramm meiner Kosten?**  
Wir benötigen mindestens 2 Monate Kostendaten, bevor wir ein Diagramm rendern können, um Sie bei der Budgeterstellung zu unterstützen.

**Warum kann ich kein Budget für ein soeben erstelltes Abonnement festlegen?**  
Nach der Erstellung eines Abonnements dauert die Verarbeitung der Daten 24-48 Stunden, bevor sie ein Budget dafür festlegen.

**Budget-API-Ressourcen**

- [Budgets-API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Stellt Vorgänge zum Erstellen und Aktualisieren von Budgets bereit. Mithilfe der Budgets-API können Sie einen Budgetschwellenwert festlegen und mehrere Warnungen so konfigurieren, dass sie ausgelöst werden, wenn Sie sich diesem Schwellenwert nähern. Benachrichtigungen können eine E-Mail oder eine Azure-Aktionsgruppe zum Ausführen der Automatisierung auslösen. Hinweis: Das Filtern für diese API entspricht nicht der Abfrage-API-Filterung/-Dimensionen.
- [Budgets-API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Erstellen Sie Budgets mit höheren Kostenfilterfunktionen als v1. Die Filterung richtet sich nach dem Vertrag, der in unseren Abfrage- und Dimensions-APIs verwendet wird. Dies ist die empfohlene Budgets-API für die weitere Verwendung.
- [Dimensionen](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Stellt Vorgänge bereit, um unterstützte Dimensionen für Ihre Verwendung in einer Vielzahl von Bereichen abzurufen. Mithilfe der Dimensions-API können Sie eine Liste von Dimensionen abrufen, die als Eingaben zum Generieren von Abfragen mit der Abfrage-API verwendet werden können.
- [Abfrage](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Stellt Vorgänge bereit, um aggregierte Kosten- und Nutzungsdaten basierend auf der von Ihnen bereitgestellten Abfrage abzurufen. Mithilfe der Abfrage-API können Sie die gewünschte Filterung, Sortierung und Gruppierung für alle verfügbaren Dimensionen angeben (auf die über die Dimensions-API zugegriffen wird).

**Prognostizierte Kosten**

**Warum werden in der Kostenanalyse keine Prognosen für meine Kosten angezeigt?**  
Es gibt mehrere Gründe, warum die Prognoseprojektion für Sie in der Kostenanalyse fehlen könnte, einige davon sind wie folgt:

1. Wenn Ihre Kostendaten weniger als 10 Tage alt sind, wird das Prognosediagramm nicht geladen. Das Modell benötigt mindestens 10 Tage aktueller Kostendaten für genaue Projektionen.
2. Wenn Sie historische Datumsangaben ausgewählt haben, wird das Prognosediagramm nicht angezeigt. Wählen Sie einen Datumsbereich mit zukünftigen Datumsangaben für das anzuzeigende Prognosediagramm aus.
3. Wenn Ihr Konto mehrere Währungen hat, werden im Prognosediagramm nur Kosten für "Alle Kosten in USD" projiziert.

**Warum ändert sich die Prognose nicht, wenn ich Änderungen an meinen Ressourcen vorn habe?**  
Das Prognosemodell erfordert einige Tage, um Änderungen am Konto zu berücksichtigen, und es werden keine sofortigen Projektionen basierend auf Ressourcenänderungen vorgenommen.  
Bei größeren Schritten zur Erhöhung oder Verringerung der Ressourcen dauert das Modell etwas länger, um sich an diese Änderungen anzupassen, um Anomalien rechnung zu tragen.

**Warum steigt meine Prognose, nachdem ich eine Reservierung oder einen Marketplace-Kauf getätigt habe?**  
Das Prognosemodell berücksichtigt Ihre "Ist-Kosten" und berücksichtigt nicht die Nutzung und den Kauf separat. Bei einem einmaligen Kauf verringert das Modell die Projektionen nach 10 Tagen, um den plötzlichen Anstieg der Kosten zu berücksichtigen.

**Ich möchte Prognosen für eine einzelne Dimension anzeigen (z. B. Meter)**  
Prognose unterstützt derzeit Gesamtkostenprognosen und nicht für einzelne Meter. Wenn also eine Dimension nach "gruppiert" wird, werden die Projektionen für die Summe aller Elemente in der Dimension sein.

**Empfohlene Dokumentationen**

- [Was ist Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysieren Ihrer Kosten und Ausgaben](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Untersuchen und Analysieren von Kosten mithilfe der Kostenanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Preise](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kosten in der Kostenanalyse überprüfen](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videolernprogramm: Erstellen eines Budgets im Azure-Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Voraussetzungen für das Anzeigen und Anpassen von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Erstellen und Verwalten von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurieren der Automatisierung mit der Azure Action Groups and Budgets-API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Verwenden von Kostenwarnungen zum Überwachen von Nutzung und Ausgaben](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für das Kostenmanagement](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Lernprogrammvideos**

- [Erstellen eines Budgets im Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Verwalten von Kosten mit der Budgets-API und Aktionsgruppen](https://go.microsoft.com/fwlink/?linkid=2147038)