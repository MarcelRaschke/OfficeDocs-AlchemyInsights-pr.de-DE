---
title: Fehler beim Überprüfen des Zugriffstokens während Desktop Analytics Beim Boarding
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000657"
- "2536"
ms.openlocfilehash: 54f24bf5a5dd8cbcf8b2998984046f7daef93d52
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66378111"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler "Fehler beim Überprüfen des Zugriffstokens" während Desktop Analytics Onboarding

Dieser Fehler wird normalerweise beobachtet, wenn das Authentifizierungstoken abläuft. Bei der Aktualisierung der Seite wird das Token in der Regel aktualisiert. Dieses Problem kann jedoch weiterhin auftreten, wenn richtlinien für bedingten Zugriff auf das Konto angewendet werden, das für die Desktop Analytics verwendet wird. Sie können die Azure AD-Anmeldeprotokolle im Azure-Portal überprüfen, um festzustellen, ob Anmeldefehler für das Konto auftreten, das für Desktop Analytics Onboarding verwendet wird.

Weitere Informationen zum bedingten Zugriff finden Sie unter ["Planen der Bereitstellung für bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)".