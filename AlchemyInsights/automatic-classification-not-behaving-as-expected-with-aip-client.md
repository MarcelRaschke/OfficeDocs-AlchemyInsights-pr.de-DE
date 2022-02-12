---
title: 'AIP-Client: Die automatische Klassifizierung zeigt nicht das erwartete Verhalten'
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
- "9002266"
- "4373"
ms.openlocfilehash: 084d35e12426e738270df5b320b71ba8e34aea0c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62594545"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>AIP-Client: Die automatische Klassifizierung zeigt nicht das erwartete Verhalten

Die automatische Klassifizierung zeigt nicht das erwartete Verhalten? Verwenden Sie die folgenden empfohlenen Leitfäden:

1. Wenn Sie Probleme mit der automatischen Bezeichnung haben, lesen Sie [Konfigurieren von Bedingungen für die automatische und empfohlene Klassifizierung für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) und [Wonach die Typen von vertraulichen Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Überprüfen Sie, ob Sie nicht ordnungsgemäß konfigurierte, bereichsbezogene Richtlinien verwenden: [Konfigurieren der Azure Information Protection-Richtlinie für bestimmte Benutzer mithilfe von bereichsbezogenen Richtlinien](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Wenn die automatische Bezeichnung beim Anfügen eines mit einer Bezeichnung versehenen Dokuments in Outlook nicht funktioniert, überprüfen Sie, ob `DRMEncryptProperty` etwa nicht wie hier beschrieben definiert ist: [IRM-Registrierungseinstellungen für Sicherheit](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Wenn Sie die [integrierten Informationstypen](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) für Ihre Azure Information Protection-Richtlinie verwendet haben, überprüfen Sie, ob die Inhalte dem erwarteten Format entsprechen.
5. Vergewissern Sie sich, dass die Bezeichnung ordnungsgemäß für **Automatisch** oder **Empfohlen** konfiguriert ist. (Die **automatische** Bezeichnung steht für alle Microsoft 365-Apps zur Verfügung, während die **empfohlene** für alle Microsoft 365-Apps außer Outlook verfügbar ist.)
6. Sie können keine automatische Klassifizierung für Dokumente und E-Mails verwenden, die zuvor manuell bezeichnet oder automatisch mit einer höheren Klassifizierung gekennzeichnet wurden.  Weitere Informationen finden Sie unter [Anwenden automatischer oder empfohlener Bezeichnungen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Wenn weiterhin Probleme auftreten, rufen Sie Azure Information Protection-Clientprotokolle ab, und fügen Sie die exportierten Protokolle an Ihr Support-Ticket an. So exportieren Sie Azure Information Protection-Protokolle:
    - Öffnen Sie ein Office-Dokument oder erstellen Sie eine neue E-Mail in Outlook.
    - Klicken Sie auf **Schutz/Vertraulichkeit** > **Hilfe und Feedback**.
    - Klicken Sie auf **Protokolle exportieren**.
    - Speichern Sie die Protokolle an einem beliebigen Ort, und fügen Sie sie an Ihre Serviceanfrage an.

Weitere Informationen finden Sie unter:

- [Konfigurieren von Bedingungen für die automatische und empfohlene Klassifizierung für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Kurzanleitungen für häufige Szenarios, in denen Azure Information Protection verwendet wird](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Nachschlagen in der Azure Information Protection-Dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Informationen zu Azure Information Protection-Abonnements und -Features](https://azure.microsoft.com/pricing/details/information-protection)
- [Anforderungen für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Schnellstart-Tutorial für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection Client herunterladen](https://www.microsoft.com/download/details.aspx?id=53018)
