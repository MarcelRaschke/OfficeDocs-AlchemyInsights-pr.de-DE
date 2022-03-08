---
title: 'AIP: Richtlinien zeigen nicht das erwartete Verhalten'
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
- "9002266"
- "4780"
ms.openlocfilehash: d908149ed533f992cee852fddca42d579881fc49
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63279593"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Richtlinien zeigen nicht das erwartete Verhalten

Azure Information Protection: Zeigen Richtlinien nicht das erwartete Verhalten? In den folgenden empfohlenen Ressourcen finden Sie Leitfäden für verschiedene Probleme mit Richtlinien:

1. Wenn Probleme mit visuellen Markierungen auftreten, lesen Sie [Wann visuelle Markierungen angewendet werden](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Wenn Sie Probleme mit der automatischen Bezeichnung haben, lesen Sie [Konfigurieren von Bedingungen für die automatische und empfohlene Klassifizierung für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) und [Wonach die Typen von vertraulichen Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Wenn es Probleme mit dem nativen/Datei-Schutz gibt, lesen Sie [Datei-API-Konfiguration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Überprüfen Sie, ob Sie nicht ordnungsgemäß konfigurierte, bereichsbezogene Richtlinien verwenden: [Konfigurieren der Azure Information Protection-Richtlinie für bestimmte Benutzer mithilfe von bereichsbezogenen Richtlinien](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Wenn die automatische Bezeichnung beim Anfügen eines mit einer Bezeichnung versehenen Dokuments in Outlook nicht funktioniert, überprüfen Sie, ob DRMEncryptProperty nicht etwa wie hier beschrieben definiert ist: [IRM-Registrierungseinstellungen für Sicherheit](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Wenn weiterhin Probleme auftreten, rufen Sie Azure Information Protection-Clientprotokolle ab, und fügen Sie die exportierten Protokolle an dieses Ticket an.

1. Öffnen Sie ein Office-Dokument oder erstellen Sie eine neue E-Mail in Outlook.
2. Klicken Sie auf **Schutz/Vertraulichkeit** > **Hilfe und Feedback**.
3. Klicken Sie auf **Protokolle exportieren**.
4. Speichern Sie die Protokolle an einem beliebigen Ort, und fügen Sie sie an diese Serviceanfrage an.

Zusätzliche Ressourcen:

- [Konfigurieren einer Bezeichnung für visuelle Markierungen für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Nachschlagen in der Azure Information Protection-Dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Verwenden von Vertraulichkeitsbezeichnungen in Microsoft 365-Apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

