---
title: Fehler beim Überprüfen des Zugriffstokenfehlers während des Onboardings von Desktop Analytics
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 7bd75ccc8ef79271617796ec99feac5845aa33c0
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61942099"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler "Fehler beim Überprüfen des Zugriffstokens" beim Onboarding von Desktop Analytics

Dieser Fehler wird normalerweise beobachtet, wenn das Authentifizierungstoken abläuft. In der Regel wird beim Aktualisieren der Seite das Token aktualisiert. Dieses Problem kann jedoch weiterhin bestehen bleiben, wenn auf das Konto, das für die lokale Desktop Analytics verwendet wird, Richtlinien für bedingten Zugriff angewendet werden. Sie können die Azure AD Anmeldeprotokolle im Azure-Portal überprüfen, um festzustellen, ob Anmeldefehler für das Konto vorliegen, das für das Desktop Analytics-Onboarding verwendet wird.

Weitere Informationen zum bedingten Zugriff finden Sie unter [Planen der Bereitstellung des bedingten Zugriffs.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)