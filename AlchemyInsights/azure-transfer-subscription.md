---
title: Übertragen des Besitzes von Azure-Abrechnungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 8833c1d35d0c12ae80d13b475c1c927b125a7438
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63259001"
---
# <a name="transfer-azure-billing-ownership"></a>Übertragen des Besitzes von Azure-Abrechnungen

Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) als Administrator des Abrechnungskontos mit dem Abonnement an, das Sie übertragen möchten. Wenn Sie nicht genau wissen, ob Sie Administrator sind, oder wenn Sie ermitteln möchten, wer dies ist, lesen Sie [Ermitteln des Administrators des Abrechnungskontos](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Suchen Sie nach _Kostenverwaltung und Abrechnung_.
1. Wählen Sie im linken Bereich **Abonnements** aus. Je nach Zugriff müssen Sie möglicherweise einen Abrechnungsbereich und dann **Abonnements** oder **Azure-Abonnements** auswählen.
1. Wählen Sie **Übertragen des Besitzes von Abrechnungen** für das Abonnement, das Sie übertragen möchten.
1. Geben Sie die E-Mail-Adresse eines Benutzers ein, der ein Rechnungsadministrator des Kontos ist, das der neue Eigentümer für das Abonnement sein wird, und wählen Sie dann **Übertragungsanforderung** senden.
1. Der Benutzer erhält eine E-Mail mit Anweisungen zur Überprüfung Ihrer Übertragungsanforderung. Um die Übertragungsanforderung zu genehmigen, wählt der Benutzer den Link in der E-Mail aus und folgt den Anweisungen.

Beachten Sie, dass durch das Übertragen des Besitzes von Abrechnungen Ihres Abonnements auf das Konto eines Benutzers in einem anderen Azure AD-Mandanten alle [rollenbasierten Zugriffssteuerungen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) zur Verwaltung der Ressourcen im Abonnement dauerhaft entfernt werden. Nur der neue Eigentümer hat Zugriff auf die Verwaltung der Ressourcen im Abonnement. Weitere Informationen zum Ändern des Verzeichnisses für ein Abonnement finden Sie unter [Übertragung des Abonnements an einen Benutzer in einem anderen Azure AD-Mandanten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Wichtige Auswirkung auf Ihre Rechnungen**_: Wenn Sie den Rechnungsbesitz für ein Azure-Abonnement übertragen haben, werden Ihre Gebühren anteilig berechnet. Sie können auf die Rechnungen wie folgt zugreifen:  

1. Wählen Sie auf der Seite  [Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)  im Azure-Portal Ihr Abonnement als  [Benutzer mit Zugriff auf Rechnungen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) und dann  **Rechnungen** aus.
1. Klicken Sie auf  **Rechnung herunterladen** , um eine Kopie Ihrer PDF-Rechnung anzuzeigen. Wenn  _Nicht verfügbar_ angezeigt wird, lesen Sie  [Warum wird keine Rechnung für den letzten Abrechnungszeitraum angezeigt?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. Sie können auch die tägliche Nutzung durch Anklicken des **Abrechnungszeitraums** anzeigen, um eine PDF-Version Ihrer Rechnung sowie eine Kopie der Datei mit detaillierten täglichen Nutzungsdaten (.CSV) zu erhalten. Weitere Informationen finden Sie unter  [Abrufen von Rechnungen und Nutzungsdaten](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Empfohlene Dokumente**

- [Übertragen des Besitzes von Abrechnungen eines Azure-Abonnements auf ein anderes Konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informationen zum Übertragen des Besitzes von Abrechnungen für ein Azure-Abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Übertragen von Abonnements für Visual Studio, Microsoft Partner Network (MPN) und Pay as you go Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Übertragung des Besitzes – FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problembehandlung bei der Übertragung des Besitzes](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
