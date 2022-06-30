---
title: Anmeldung bei E-Mail nicht
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010939"
- "17696"
ms.openlocfilehash: 8286e439a0ec54d22b3c59705c62dc776f5790d9
ms.sourcegitcommit: 6bb8dd2dc45a4efe2469c9db430cd36fdb6a7fea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66504233"
---
# <a name="cant-sign-in-into-email"></a>Anmeldung bei E-Mail nicht

Wenn sich ein Benutzer nicht bei E-Mails anmelden kann:

- Stellen Sie sicher, dass sie über eine gültige Lizenz verfügen, die Exchange Online enthält. Weitere Informationen finden Sie unter [Zuweisen von Lizenzen zu Benutzern](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Die Bereitstellung des Postfachs kann bis zu 30 Minuten dauern.
- Versuchen Sie, ein "in privatem" Browserfenster zu verwenden, um sicherzustellen, dass sie ein Geschäfts-, Schul- oder Unikonto verwenden und sich anmelden `https://outlook.office.com` oder `http://portal.office.com`.
- Ein Administrator kann das Kennwort zurücksetzen, indem er zu "[**Aktive**](https://portal.office.com/adminportal/home#/users) **Benutzer** > " geht, den/die Benutzer auswählt und **"Kennwort zurücksetzen"** auswählt oder [SSPR (Self Service Password Reset)](https://passwordreset.microsoftonline.com/) verwendet, um Ihr Kennwort zurückzusetzen.
- Überprüfen Sie, ob sie sich für die mehrstufige Authentifizierung (MFA) registrieren müssen. Sicherheitsstandards, einschließlich MFA, sind für neue Mandanten aktiviert und werden für vorhandene Mandanten bereitgestellt. Weitere Informationen finden Sie unter ["Sicherheitsstandards"](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Weitere Hilfe finden [Sie unter Anmelden bei Office 365](https://docs.microsoft.com/office365/troubleshoot/sign-In/sign-in-to-office-365-azure-intune) oder [Zurücksetzen von Kennwörtern in Microsoft 365 Business](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords).