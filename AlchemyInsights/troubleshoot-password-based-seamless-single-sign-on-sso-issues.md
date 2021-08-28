---
title: Behandeln von Problemen mit kennwortbasiertem einmaligem Anmelden (Single Sign-On, SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972823"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Behandeln von Problemen mit kennwortbasiertem einmaligem Anmelden (Single Sign-On, SSO)

Informationen zu den Grundlagen des kennwortbasierten SSO finden Sie unter [Kennwortbasierte Authentifizierung mit Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurieren des kennwortbasierten SSO**

1. [Konfigurieren des kennwortbasierten einmaligen Anmeldens](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – In diesem Artikel wird ausführlicher auf die kennwortbasierte SSO-Option eingegangen. Wenn die Anwendung, die Sie hinzufügen, eine benutzerdefinierte Konfiguration erfordert und Sie kennwortbasiertes SSO verwenden müssen, ist dieser Artikel für Sie geeignet.
2. [Konfigurieren des kennwortbasierten einmaligen Anmeldens für lokale Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Anwendungsproxy unterstützt mehrere Single Sign-On-Modi. Die kennwortbasierte Anmeldung ist für Anwendungen vorgesehen, die eine Kombination aus Benutzername und Kennwort für die Authentifizierung verwenden. Wenn Sie die kennwortbasierte Anmeldung für Ihre Anwendung konfigurieren, müssen sich Ihre Benutzer einmal bei der lokalen Anwendung anmelden. Danach speichert Azure Active Directory die Anmeldeinformationen und stellt sie automatisch der Anwendung bereit, wenn Ihre Benutzer remote darauf zugreifen.
    - Sie sollten Ihre App bereits mit dem Anwendungsproxy veröffentlicht und getestet haben. Wenn nicht, führen Sie die Schritte unter Veröffentlichen von Anwendungen mithilfe des [Azure AD-Anwendungsproxys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) aus, und setzen Sie dann Ihre Konfiguration des kennwortbasierten SSO für lokale Apps fort.

Informationen zur Problembehandlung bei kennwortbasiertem einmaligem Anmelden finden Sie unter [Problembehandlung bei kennwortbasiertem einmaligem Anmelden in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
