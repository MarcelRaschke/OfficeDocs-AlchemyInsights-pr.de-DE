---
title: Übertragungsdienste – Verschieben aller RDFE-Dienste in ein anderes Abonnement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940055"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Übertragungsdienste – Verschieben aller RDFE-Dienste in ein anderes Abonnement

**Verschieben von Ressourcen**

Azure-Ressourcen können über das Azure-Portal, Azure PowerShell, Azure CLI oder die REST-API zum Verschieben von Ressourcen in ein anderes Azure-Abonnement oder eine andere Ressourcengruppe unter demselben Abonnement verschoben werden.

Bevor Sie Ressourcen verschieben können, lesen Sie:

- [Prüfliste vor dem Verschieben von Ressourcen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Dienste, die verschoben werden können](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [So überprüfen Sie die Verschiebung](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Verschiebungsanleitungen für Dienste](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Um vorhandene Ressourcen in eine andere Ressourcengruppe oder ein anderes Abonnement zu verschieben, können Sie Folgendes verwenden:

- [Azure-Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Lernprogramm: [Verschieben von Azure-Ressourcen in eine andere Ressourcengruppe oder ein anderes Abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Behandeln von Fehlern mit Azure Resource Manager**

Lesen Sie die folgenden Artikel, um mehr über einige häufige Azure-Bereitstellungsfehler zu erfahren und Informationen zu deren Behebung zu erhalten. Wenn Sie den Fehlercode für den Bereitstellungsfehler nicht finden können, lesen [Sie "Fehlercode suchen".](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Problembehandlung bei Bereitstellungsfehlern](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Problembehandlung beim Verschieben von Azure-Ressourcen in eine neue Ressourcengruppe oder ein neues Abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Beachten Sie, dass Sie Ihr Abonnement konvertieren müssen, wenn Sie Ihr Azure-Abonnement aktualisieren möchten, z. B. von kostenlos zu kostenpflichtig wechseln.

- Informationen zum Upgrade einer kostenlosen Testversion finden Sie unter [Upgrade Ihrer kostenlosen Testversion oder Ihres Microsoft Imagine Azure-Abonnements auf "Pay-As-You-Go".](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Informationen zum Ändern eines Pay-as-You-Go-Kontos finden Sie unter [Ändern Ihres Azure Pay-As-You-Go-Abonnements in ein anderes Angebot.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**So fügen Sie Ihrem Azure Active Directory Mandanten ein Azure-Abonnement hinzu oder ordnen es zu:**

1. Melden Sie sich an, und wählen Sie das Abonnement aus, das Sie verwenden möchten, auf der [Seite "Abonnements" im Azure-Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Wählen Sie **"Verzeichnis ändern"** aus.
3. Überprüfen Sie alle angezeigten Warnungen, und wählen Sie dann **Ändern** aus.
4. Das Verzeichnis wird für das Abonnement geändert, und Sie erhalten eine Erfolgsmeldung.
5. Verwenden  Sie die Verzeichnis-Switcher, um zu Ihrem neuen Verzeichnis zu wechseln. Es kann bis zu 10 Minuten dauern, bis alles ordnungsgemäß angezeigt wird.

**Empfohlene Dokumente**

- [Übertragen des Besitzes eines Azure-Abonnements](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Verschieben von Ressourcen in eine neue Ressourcengruppe oder ein neues Abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Verwalten von Ressourcen mithilfe des Azure-Portals](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
