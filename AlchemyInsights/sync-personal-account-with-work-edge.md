---
title: Ermöglichen Sie es einem Benutzer, ein persönliches Konto mit dem Geschäftskonto in Microsoft Edge zu synchronisieren
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: cbbb165a6ad6cffc8193f6ed30ec2d0bf5bbb5c1
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65734808"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Ermöglichen Sie es einem Benutzer, ein persönliches Konto mit dem Geschäftskonto in Microsoft Edge zu synchronisieren

Stellen Sie sicher, dass Sie die folgenden Kriterien erfüllen:

- Enterprise State Roaming ist im Azure Active Directory Admin Center aktiviert, was ein Abonnement für Azure Active Directory Premium oder Enterprise Mobility + Security (EMS) erfordert. Weitere Informationen finden Sie unter [Aktivieren von Enterprise State Roaming in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable).
- Eines oder beide der folgenden Kriterien sind erfüllt:
  - Der Azure Information Protection-Dienst ist für Ihren Mandanten aktiviert. Weitere Informationen finden Sie unter [Aktivieren des Azure Rights Management-Schutzes über das Microsoft 365 Admin Center](https://docs.microsoft.com/azure/information-protection/activate-office365).
  - Die ESR-Funktion (Azure Active Directory Enterprise State Roaming) ist für jeden Benutzer oder Mandanten aktiviert. Weitere Informationen finden Sie unter [Was ist Enterprise State Roaming?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview).

Wenn AIP und ESR deaktiviert sind, werden die Benutzer in einer Fehlermeldung darüber informiert, dass die Synchronisierung für ihre Konten nicht verfügbar ist.
