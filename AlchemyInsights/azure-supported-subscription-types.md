---
title: Unterstützte Abonnementtypen
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
- "6675"
ms.openlocfilehash: e26be1a9da3d7ed83e18d298db3e704966bfd767
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63259037"
---
# <a name="supported-subscription-types"></a>Unterstützte Abonnementtypen

Bitte überprüfen Sie die unterstützten Abonnementtypen, um fortzufahren.

[Unterstützte Abonnementtypen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Übertragen des Besitzes von Abrechnungen**

Azure-Portal als [Konto-Administrator](https://ms.portal.azure.com/) des Abrechnungskontos mit dem Abonnement, das Sie übertragen möchten

- Suchen nach **Kostenverwaltung + Abrechnung**. Wählen Sie im linken Bereich **Abonnements** aus. Je nach Zugriff müssen Sie möglicherweise einen Abrechnungsumfang und dann **Abonnements** oder **Azure-Abonnements** auswählen.
- Wählen Sie „Übertragen des Besitzes von Abrechnungen“ für das Abonnement, das Sie übertragen möchten.
- Geben Sie die E-Mail-Adresse eines Benutzers ein, der ein Rechnungsadministrator des Kontos ist, das der neue Eigentümer für das Abonnement sein wird, und wählen Sie dann **Übertragungsanforderung** senden 
- Der Benutzer erhält eine E-Mail mit Anweisungen zur Überprüfung Ihrer Übertragungsanforderung. Um die Übertragungsanforderung zu genehmigen, wählt der Benutzer den Link in der E-Mail aus und folgt den Anweisungen.

Hinweis: Wenn Sie den Besitz von Abrechnungen Ihres Abonnements auf das Konto eines Benutzers in einem anderen Azure AD-Mandanten übertragen, werden alle [rollenbasierten Zugriffssteuerungen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) zur Verwaltung der Ressourcen im Abonnement dauerhaft entfernt. Nur der neue Eigentümer hat Zugang zur Verwaltung der Ressourcen im Abonnement. Weitere Informationen finden Sie unter [Übertragung des Abonnements an einen Benutzer in einem anderen Azure AD-Mandanten](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Übertragen des Besitzes von Abonnements**

Bei der Übertragung des Besitzes von Abonnements verliert die rollenbasierte Zugriffssteuerung (RBAC) zur Verwaltung von Ressourcen im Abonnement ihren Zugriff. Weitere Informationen über das Hinzufügen eines bestehenden Abonnements zu einem Mandanten finden Sie unter [Zuordnen oder Hinzufügen eines Azure-Abonnements zu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Die Übertragung von Abonnements mit einem bestehenden offenen Betrag aus dem aktuellen Abrechnungszyklus wird nicht auf das neue Zahlungsinstrument im neuen Konto übertragen. Die einzigen Informationen, die den Benutzern in einem neuen Konto zur Verfügung stehen, sind die Kosten des letzten Monats für Ihr Abonnement. Der Rest der Nutzungs- und Abrechnungshistorie wird nicht mit dem Abonnement übertragen.
- Die Übertragung des Besitzes von Abrechnungen für Enterprise Agreement (EA)-Abonnements wird derzeit nur im Enterprise Agreement-Portal unterstützt.
- Das Übertragen eines kreditorientierten Abonnements wie Visual Studio, BizSpark, Microsoft Partner Network auf einen neuen Benutzer erfordert eine Visual Studio/Microsoft-Partnernetzwerklizenz, um die Übertragungsanforderung anzunehmen
- Alle Ressourcen wie virtuelle Maschinen, Datenträger und Websites werden erfolgreich auf das neue Konto übertragen. Die folgenden Ressourcen könnten bei einer mandantenübergreifenden Abonnementübertragung betroffen sein:

**Azure AD Domain Services**

Azure Key Vaults

- [SQL-bezogene Benutzer und Datenbanken](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) könnten betroffen sein, insbesondere wenn der Kunde eine Azure Active Directory bezogene Authentifizierung verwendet
- **App-Dienste**, die mit Azure Active Directory-Authentifizierung konfiguriert sind, könnten beeinträchtigt werden
- **Visual Studio-Team** Dienstleistungskonten, die mit Azure-Abonnements verbunden sind, können vorübergehend den Zugriff verlieren, wenn das verbundene Azure-Abonnement gekündigt wird

**Empfohlene Dokumente**

Schritte nach dem Akzeptieren des Besitzes der Abrechnung:

- Um den Besitz von Abrechnungen beizubehalten, aber die Art Ihres Abonnements zu ändern, siehe [Ihr Azure-Abonnement zu einem anderen Angebot wechseln](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Übertragen von Abonnements für Visual Studio, Microsoft Partner Network (MPN) und Pay as you go Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Übertragung des Besitzes von Abrechnungen für Enterprise Agreement (EA)-Abonnements](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Übertragung des Besitzes – FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problembehandlung bei der Übertragung des Besitzes](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)