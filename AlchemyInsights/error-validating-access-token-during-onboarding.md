---
title: Fehler beim Überprüfen des Zugriffstokenfehlers während des Onboardings von Desktop Analytics
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7df7e7e27b0bb0e5a50c1196578881fb8b520818
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63266381"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler "Fehler beim Überprüfen des Zugriffstokens" beim Onboarding von Desktop Analytics

Dieser Fehler wird normalerweise beobachtet, wenn das Authentifizierungstoken abläuft. In der Regel wird beim Aktualisieren der Seite das Token aktualisiert. Dieses Problem kann jedoch weiterhin bestehen bleiben, wenn auf das Konto, das für die lokale Desktop Analytics verwendet wird, Richtlinien für bedingten Zugriff angewendet werden. Sie können die Azure AD-Anmeldeprotokolle im Azure-Portal überprüfen, um festzustellen, ob Anmeldefehler für das Konto vorliegen, das für das Desktop Analytics-Onboarding verwendet wird.

Weitere Informationen zum bedingten Zugriff finden Sie unter [Planen der Bereitstellung des bedingten Zugriffs](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).