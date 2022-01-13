---
title: Warum ist die Schaltfläche "Budget hinzufügen" für mich deaktiviert?
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 9d8872cc7b25b02b88485e7ac66d2bb79e80fdb1
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61865092"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Warum ist die Schaltfläche "Budget hinzufügen" für mich deaktiviert?

Um ein Budget zu erstellen, benötigen Sie eine der folgenden Berechtigungen:

- Verwaltungsgruppe, Abonnement, Ressourcengruppenbereiche
- Kostenverwaltungsmitwirkender
- Besitzer
- Contributor
- nur Enterprise Kunde: Registrierung, Abteilung, Kontobereiche
- Registrierungsadministrator (budget at Enrollment scope festlegen)
- Abteilungsadministrator (Budget auf Abteilungsbereich festlegen)
- Kontobesitzer (Budget auf Kontoebene festlegen)
- Nur moderner Kundenvertrag: Abrechnungskonto, Abrechnungsprofil, Rechnungsabschnittsbereiche
- Ersteller eines Azure-Abonnements

**Ich habe ein Budget erstellt, als meine Kosten für den aktuellen Monat bereits über dem Budget lag. Warum habe ich keine Warnung erhalten?**  
Wenn Sie einen bestimmten Kostenschwellenwert bereits überschritten haben, wenn Sie ein Budget erstellen, wird diese Warnung nicht ausgelöst. Sobald ein neuer Zyklus beginnt, wird die Warnung ausgelöst, wenn Sie den Schwellenwert überschreiten.

**Wann sollte ich davon ausgehen, dass ich eine Warnung erhalte, nachdem ich einen meiner definierten Schwellenwerte für Budgetwarnungen überschritten habe?**  
Budgets werden alle 4 Stunden ausgewertet. Es dauert mindestens 8 Stunden, bis Nutzungsdaten das Budgetsystem erreichen. In diesem Fall kann es bis zu 12 Stunden dauern, bis Warnungen ausgelöst werden, nachdem Sie einen Schwellenwert überschritten haben.

**Warum ist die Schaltfläche "Startdatum" deaktiviert, wenn ich einen Zurücksetzungszeitraum für den Monat oder den Abrechnungsmonat auswähle?**  
Die Budgets werden an den aktuellen Kalendermonat oder den aktuellen Abrechnungszeitraum angepasst (in dem Fall, in dem der Abrechnungsmonat ausgewählt ist). Daher füllen wir diesen Wert vorab für Sie auf.

**Warum wird in der Budgeterstellung kein Diagramm meiner Kosten angezeigt?**  
Wir benötigen mindestens zwei Monate Kostendaten, bevor wir ein Diagramm rendern können, um Sie bei der Budgeterstellung zu unterstützen.

**Warum kann ich kein Budget für ein soeben erstelltes Abonnement festlegen?**  
Nach der Erstellung eines Abonnements dauert die Verarbeitung der Daten 24-48 Stunden, bevor ein Budget dafür festgelegt wird.

**Budget-API-Ressourcen**

- [Budget-API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Stellt Vorgänge zum Erstellen und Aktualisieren von Budgets bereit. Mithilfe der Budget-API können Sie einen Budgetschwellenwert festlegen und mehrere Warnungen konfigurieren, die ausgelöst werden, wenn Sie sich diesem Schwellenwert nähern. Warnungen können eine E-Mail oder eine Azure-Aktionsgruppe auslösen, um automatisierungsfähig zu werden. Hinweis: Die Filterung für diese API entspricht nicht der Filterung/Dimensionen der Abfrage-API.
- [Budget-API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Erstellen Sie Budgets mit höheren Kostenfilterfunktionen als v1. Die Filterung richtet sich nach dem Vertrag aus, der in unseren Abfrage- und Dimensions-APIs verwendet wird. Dies ist die empfohlene Budget-API für die weitere Verwendung.
- [Dimensionen:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Stellt Vorgänge bereit, um unterstützte Dimensionen für Ihre Verwendung in einer Vielzahl von Bereichen abzurufen. Mithilfe der Dimensions-API können Sie eine Liste der Dimensionen abrufen, die als Eingaben zum Generieren von Abfragen mit der Abfrage-API verwendet werden können.
- [Abfrage:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Stellt Vorgänge bereit, um aggregierte Kosten- und Nutzungsdaten basierend auf der von Ihnen bereitgestellten Abfrage abzurufen. Mithilfe der Abfrage-API können Sie die gewünschte Filterung, Sortierung und Gruppierung nach allen verfügbaren Dimensionen angeben (auf die über die Dimensions-API zugegriffen wird).

**Prognostizierte Kosten**

**Warum werden in der Kostenanalyse keine Vorhersagen für meine Kosten angezeigt?**  
Es gibt mehrere Gründe, warum die Prognostizierung in der Kostenanalyse für Sie möglicherweise fehlt. Einige davon sind wie folgt:

1. Wenn Ihre Kostendaten weniger als 10 Tage alt sind, wird das Prognosediagramm nicht geladen. Das Modell erfordert mindestens 10 Tage der aktuellen Kostendaten für genaue Projektionen.
2. Wenn Sie historische Datumsangaben ausgewählt haben, ist das Prognosediagramm nicht sichtbar. Wählen Sie einen Datumsbereich mit zukünftigen Datumsangaben für das anzuzeigende Prognosediagramm aus.
3. Wenn Ihr Konto mehrere Währungen aufweist, projiziert das Prognosediagramm nur die Kosten für "Alle Kosten in USD".

**Warum ändert sich die Prognose nicht, wenn ich Änderungen an meinen Ressourcen vorstelle?**  
Das Prognosemodell erfordert ein paar Tage, um Änderungen am Konto zu berücksichtigen, und erstellt keine sofortigen Projektionen basierend auf änderungen an Ressourcen  
Bei größeren Schritten zur Erhöhung oder Reduzierung von Ressourcen dauert es etwas länger, bis das Modell sich an diese Änderungen anpasst, um Anomalien zu berücksichtigen.

**Warum erhöht sich meine Prognose, nachdem ich eine Reservierung oder einen Marketplace-Kauf vorgenommen habe?**  
Das Prognosemodell berücksichtigt Ihre "aktuellen Kosten" und berücksichtigt die Nutzung und den Kauf nicht separat. Bei einem einmaligen Kauf verringert das Modell die Projektionen nach 10 Tagen, um die plötzliche Kostensteigerung zu berücksichtigen.

**Ich möchte Vorschauen für eine einzelne Dimension anzeigen (z. B. Meter)**  
Die Prognose unterstützt derzeit Projektionen der Gesamtkosten und nicht für einzelne Meter. Wenn eine Dimension "gruppiert nach" ist, sind die Projektionen daher für die Summe aller Elemente in der Dimension

**Empfohlene Dokumentationen**

- [Was ist Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysieren Sie Ihre Kosten und Ausgaben](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Erkunden und Analysieren von Kosten mit kostenanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Preise](https://azure.microsoft.com/services/cost-management/#pricing)
- [Überprüfen der Kosten in der Kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videolernprogramm: Erstellen eines Budgets im Azure-Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Voraussetzungen für das Anzeigen und Anpassen von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Erstellen und Verwalten von Budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurieren der Automatisierung mit der Azure-Aktionsgruppen- und Budget-API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Verwenden von Kostenwarnungen zur Überwachung von Nutzung und Ausgaben](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bewährte Methoden für die Kostenverwaltung](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Lernprogrammvideos**

- [Erstellen eines Budgets im Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Verwalten von Kosten mit der Budget-API und Aktionsgruppen](https://go.microsoft.com/fwlink/?linkid=2147038)