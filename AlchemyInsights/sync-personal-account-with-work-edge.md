---
title: Ermöglichen Sie es einem Benutzer, ein persönliches Konto mit dem Geschäftskonto in Microsoft Edge zu synchronisieren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: ad4b64c4bb50f50d4ab9fa47bb37228dce538e6d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317277"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Ermöglichen Sie es einem Benutzer, ein persönliches Konto mit dem Geschäftskonto in Microsoft Edge zu synchronisieren

Stellen Sie sicher, dass Sie die folgenden Kriterien erfüllen:

- Enterprise State Roaming ist im Azure Active Directory Admin Center aktiviert, was ein Abonnement für Azure Active Directory Premium oder Enterprise Mobility + Security (EMS) erfordert. Weitere Informationen finden Sie unter [Aktivieren von Enterprise State Roaming in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable).
- Eines oder beide der folgenden Kriterien sind erfüllt:
    - Der Azure Information Protection-Dienst ist für Ihren Mandanten aktiviert. Weitere Informationen finden Sie unter [Aktivieren des Azure Rights Management-Schutzes über das Microsoft 365 Admin Center](https://docs.microsoft.com/azure/information-protection/activate-office365).
    - Die ESR-Funktion (Azure Active Directory Enterprise State Roaming) ist für jeden Benutzer oder Mandanten aktiviert. Weitere Informationen finden Sie unter [Was ist Enterprise State Roaming?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview).

Wenn AIP und ESR deaktiviert sind, werden die Benutzer in einer Fehlermeldung darüber informiert, dass die Synchronisierung für ihre Konten nicht verfügbar ist.
