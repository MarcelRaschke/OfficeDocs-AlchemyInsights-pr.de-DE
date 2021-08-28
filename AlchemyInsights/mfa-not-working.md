---
title: Probleme mit MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098601"
---
# <a name="issues-with-azure-mfa"></a>Probleme mit Azure MFA
Es gibt einige Dinge zu überprüfen, ob sich Benutzer nicht mithilfe der mehrstufigen Authentifizierung (MFA) anmelden können.

1. Der betroffene Benutzer kann im Azure Active Directory Portal blockiert werden. Wenn dies der Fall ist, werden Authentifizierungsversuche für diesen bestimmten Benutzer automatisch abgelehnt. [Führen Sie die Schritte in diesem Artikel aus, um die Blockierung aufzuheben.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Wenn die Blockierung des Benutzers nicht hilfreich war oder der Benutzer nicht blockiert ist, können Sie versuchen, die MFA für den Benutzer zurückzusetzen, und er durchläuft den Registrierungsprozess erneut. [Führen Sie die Schritte in diesem Artikel aus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Wenn Sie MFA zum ersten Mal aktiviert haben und sich Ihre Benutzer nicht bei Nicht-Browser-Clients wie Outlook, Skype usw. anmelden können, ist möglicherweise ADAL (Active Directory-Authentifizierungsbibliothek) in Ihrem O365-Abonnement nicht aktiviert. In diesem Fall müssen Sie eine Verbindung mit Exchange Online PowerShell herstellen und dieses Cmdlet ausführen: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*