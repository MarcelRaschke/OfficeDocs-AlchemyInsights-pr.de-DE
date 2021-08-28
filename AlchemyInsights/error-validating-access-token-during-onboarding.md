---
title: Fehler beim Überprüfen des Zugriffstokenfehlers während des Onboardings von Desktop Analytics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946614"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler "Fehler beim Überprüfen des Zugriffstokens" beim Onboarding von Desktop Analytics

Dieser Fehler wird normalerweise beobachtet, wenn das Authentifizierungstoken abläuft. In der Regel wird beim Aktualisieren der Seite das Token aktualisiert. Dieses Problem kann jedoch weiterhin bestehen bleiben, wenn auf das Konto, das für die lokale Desktop Analytics verwendet wird, Richtlinien für bedingten Zugriff angewendet werden. Sie können die Azure AD-Anmeldeprotokolle im Azure-Portal überprüfen, um festzustellen, ob Anmeldefehler für das Konto vorliegen, das für das Desktop Analytics-Onboarding verwendet wird.

Weitere Informationen zum bedingten Zugriff finden Sie unter [Planen der Bereitstellung des bedingten Zugriffs.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)