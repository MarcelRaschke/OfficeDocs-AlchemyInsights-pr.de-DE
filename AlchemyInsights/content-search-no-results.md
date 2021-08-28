---
title: Inhaltssuche keine Ergebnisse
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
- "9000661"
- "2527"
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058001"
---
# <a name="no-results-from-content-searchexports"></a>Keine Ergebnisse der Inhaltssuche/-exporte

Probleme mit der Inhaltssuche/-exporte, die keine Daten zurückgeben, können auf einen bestimmten Compliancesicherheitsfilter zurückzuführen sein, der von einem bestimmten Administrator eingerichtet und nicht an alle Administratoren kommuniziert wurde.

Um dies zu beheben, überprüfen Sie, ob Compliancesicherheitsfilter vorhanden sind, die dies verursachen können:
1. Verbinden zu Security and Compliance Center PowerShell
2. Führen Sie die folgenden Commandlets aus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter - Organisations-$org