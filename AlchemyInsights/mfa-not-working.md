---
title: Probleme mit MFA
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 461c127de45a4186a16e3746ae6d58cbd16a4d04
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62620405"
---
# <a name="issues-with-azure-mfa"></a>Probleme mit Azure MFA
Es gibt einige Dinge zu überprüfen, ob sich Benutzer nicht mithilfe der mehrstufigen Authentifizierung (MFA) anmelden können.

1. Der betroffene Benutzer kann im Azure Active Directory Portal blockiert werden. Wenn dies der Fall ist, werden Authentifizierungsversuche für diesen bestimmten Benutzer automatisch abgelehnt. [Führen Sie die Schritte in diesem Artikel aus, um die Blockierung aufzuheben.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Wenn die Blockierung des Benutzers nicht hilfreich war oder der Benutzer nicht blockiert ist, können Sie versuchen, die MFA für den Benutzer zurückzusetzen, und er durchläuft den Registrierungsprozess erneut. [Führen Sie die Schritte in diesem Artikel aus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Wenn Sie MFA zum ersten Mal aktiviert haben und sich Ihre Benutzer nicht bei Nicht-Browser-Clients wie Outlook, Skype usw. anmelden können, ist möglicherweise ADAL (Active Directory-Authentifizierungsbibliothek) in Ihrem O365-Abonnement nicht aktiviert. In diesem Fall müssen Sie eine Verbindung mit Exchange Online PowerShell herstellen und dieses Cmdlet ausführen: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*