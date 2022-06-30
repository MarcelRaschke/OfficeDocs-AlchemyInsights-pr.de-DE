---
title: Probleme mit MFA
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000557"
- "2417"
ms.openlocfilehash: 20cf29f31f29143e966e5b030c6b8346b2bd485d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66351975"
---
# <a name="issues-with-azure-mfa"></a>Probleme mit Azure MFA
Es gibt einige Dinge zu überprüfen, ob sich Benutzer nicht mithilfe der mehrstufigen Authentifizierung (Multi-Factor Authentication, MFA) anmelden können.

1. Der betroffene Benutzer kann im Azure Active Directory-Portal blockiert werden. Wenn dies der Fall ist, werden Authentifizierungsversuche für diesen bestimmten Benutzer automatisch verweigert. [Führen Sie die Schritte in diesem Artikel aus, um die Blockierung aufzuheben.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Wenn das Aufheben der Blockierung des Benutzers nicht geholfen hat oder der Benutzer nicht blockiert wird, können Sie versuchen, die MFA für den Benutzer zurückzusetzen, und der Benutzer durchläuft den Registrierungsprozess erneut. [Führen Sie die Schritte in diesem Artikel aus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Wenn Sie MFA zum ersten Mal aktiviert haben und Sich Ihre Benutzer nicht bei Nicht-Browser-Clients wie Outlook, Skype usw. anmelden können, ist möglicherweise ADAL (Active Directory-Authentifizierungsbibliothek) in Ihrem O365-Abonnement nicht aktiviert. In diesem Fall müssen Sie eine Verbindung mit Exchange Online Powershell herstellen und dieses Cmdlet ausführen: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*