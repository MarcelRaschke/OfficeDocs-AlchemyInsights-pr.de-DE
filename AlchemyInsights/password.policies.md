---
title: Kennwortrichtlinien
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004595"
- "9277"
ms.date: 03/11/2021
ms.openlocfilehash: 01b17e52ba3124bf622bd853fd90249d3718014c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66256006"
---
# <a name="password-policies"></a>Kennwortrichtlinien

**Ich habe Probleme mit der Kennwortrichtlinie für einen Benutzer**

- Die Kennwortrichtlinie für einen Benutzer hängt davon ab, ob der Benutzer nur in der Cloud oder lokal ist.
- Nur Cloudbenutzer müssen ein Kennwort auswählen, das die Anforderungen in diesem Artikel erfüllt: [Kennwortrichtlinien, die nur für Cloudbenutzerkonten gelten](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokale Benutzer müssen ein Kennwort auswählen, das die lokalen Anforderungen erfüllt. Wenn ein lokaler Benutzer sein Kennwort nicht festlegen kann, überprüfen Sie Ihre lokalen Anforderungen.

**Ich weiß nicht, wie ich Kennwortablaufrichtlinien festlegen oder überprüfen kann.**

- Sie können die Ablaufrichtlinie für Cloudbenutzer in Ihrem Mandanten mithilfe von PowerShell festlegen und überprüfen. Befolgen Sie die Anweisungen in diesem Artikel: [Festlegen oder Überprüfen der Kennwortrichtlinien mithilfe von PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Die Kennwortablaufrichtlinie für lokale Benutzer wird in Ihrem lokalen AD festgelegt.

**Weitere hilfreiche Links:**
- [Erste Schritte mit Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Problembehandlung bei vom Administrator initiierter Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
