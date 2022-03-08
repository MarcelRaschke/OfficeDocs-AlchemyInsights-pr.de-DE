---
title: 2681-Angriffssimulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: ba5c8858dc287d742ae72cd6dff47beb65afae20
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63272789"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angriffssimulator in Microsoft 365

- Fehlt Ihnen der Angriffssimulator? Der Angriffssimulator erfordert **Microsoft Defender für Office 365 Plan 2** oder **Office 365 Enterprise E5**. Der Angriffssimulator ist **nicht** in Microsoft Defender für Office 365 Plan 1, Office 365 Enterprise E3 oder Microsoft 365 Apps for Business-Abonnements enthalten.

- Das Konto, das Sie zum Starten simulierter Angriffe verwenden, erfordert globale Administrator- oder Sicherheitsadministratorberechtigungen und mehrstufige Authentifizierung (Multi-Factor Authentication, MFA). Weitere Informationen zu den Anforderungen des Angriffssimulators finden Sie in [diesem Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Wichtige Dinge, die Sie über **Brute Force Password-Angriffssimulationen** wissen müssen:

  - Wenn für das Zielkonto MFA aktiviert ist und das Kennwort richtig erraten wurde, wird das Konto nicht als kompromittiert angezeigt (der zweite Authentifizierungsfaktor ist unvollständig).

  - Die Kennwortdatei darf nicht größer als 10 MB sein. Verwenden Sie ein Kennwort pro Zeile, und fügen Sie eine leere Zeile (Wagenrücklauf) hinter dem letzten Kennwort in der Liste ein.

- Wichtige Dinge, die Sie über **Spear Phishing** Attach-Simulationen wissen müssen:

  - Standardmäßig können Sie keinen benutzerdefinierten Wert für die URL des **Phishing-Anmeldeservers** angeben.

  - Wenn ein Empfänger [das Add-In "Nachricht melden"](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) zum Melden der Nachricht als Phishing verwendet, erhalten Sie möglicherweise keine Warnungen für die Nachricht (da es sich um einen simulierten Angriff handelt).

- Berichte: Nachdem der simulierte Angriff abgeschlossen ist, können Sie auf **"Angriffsdetails"** klicken, um den Bericht anzuzeigen.

- Ausführliche Anweisungen und neue Features im Angriffssimulator finden Sie unter ["Angriffssimulator" in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
