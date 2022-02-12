---
title: Migration von AIP zu MIP/einheitlichen Bezeichnungen im Compliance Center
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
- "9002278"
- "5114"
ms.openlocfilehash: 704c01e08cb5ab1ae30dd634fba9004de0baf5bf
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62601959"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migration von AIP zu MIP/einheitlichen Bezeichnungen im Compliance Center

Um von AIP-Bezeichnungen zu einheitlichen Bezeichnungen im Security & Compliance Center zu migrieren, gehen Sie folgendermaßen vor:

**Aktivieren Sie den Schutz über das Azure-Portal**

1. Wenn Sie dies noch nicht getan haben, öffnen Sie ein neues Browserfenster, und [melden Sie sich beim Azure-Portal an](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navigieren Sie zum Blatt **Azure Information Protection**. Klicken Sie z. B. im Hubmenü auf **Alle Dienste**, und beginnen Sie mit der Eingabe von **Informationen** im Feld "Filter". Wählen Sie **Azure Information Protection** aus. Wenn Sie bisher noch nicht auf das Blatt "Azure Information Protection" zugegriffen haben, lesen Sie die einmaligen [zusätzlichen Schritte](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time), um dieses Blatt zum Portal hinzuzufügen. Um das Blatt "Azure Information Protection" zu öffnen, müssen Sie über einen [Azure Information Protection Premium-Plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) oder einen Office 365-Plan verfügen, der die Rechteverwaltung umfasst. Wenn Sie über eines dieser Abonnements verfügen, aber eine Nachricht erhalten, dass kein gültiges Abonnement gefunden wird, [wenden Sie sich an den Microsoft-Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support), oder verwenden Sie unsere Standardsupportkanäle.

2. Suchen Sie die Menüoptionen **Verwalten**, und wählen Sie **Schutzaktivierung** aus. Klicken Sie auf **Aktivieren**, und bestätigen Sie dann Ihre Aktion. Nach Abschluss der Aktivierung wird auf der Informationsleiste **Aktivierung erfolgreich abgeschlossen** angezeigt.

**Migrieren von Azure Information Protection-Bezeichnungen zum Office 365 Security & Compliance Center**

1. Stellen Sie sicher, dass Sie als Benutzer mit globalen Administratorberechtigungen angemeldet sind.

2. Navigieren Sie zum Blatt **Azure Information Protection**.

3. Wählen Sie aus der Menüoption **Verwalten** die Option **Einheitliche Bezeichnungen** aus.

4. Klicken Sie auf dem Blatt **Azure Information Protection – Einheitliche Bezeichnungen** auf **Aktivieren**, und folgen Sie den Onlineanweisungen.

**Hinweis**: Vergewissern Sie sich, dass Sie über die entsprechenden Berechtigungen verfügen, bevor Sie die Security & Compliance Center-Migration aktivieren. Weitere Informationen finden Sie in diesen Artikeln:

1. [Benötigt man globale Administratorrechte, um Azure Information Protection zu konfigurieren, oder kann ich das an andere Administratoren delegieren?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Wichtige Informationen über administrative Rollen nach der Migration zum Security & Compliance Center](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Weitere Informationen über die Migration von AIP zu einheitlichen Bezeichnungen zum Security & Compliance Center finden Sie unter [Migrieren von Bezeichnungen](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
