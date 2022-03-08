---
title: Konfigurieren und Anpassen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: ae53bd2b3ef377fe3b7d26c09e209039a091b520
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63278261"
---
# <a name="configure-and-customize-applications"></a>Konfigurieren und Anpassen von Anwendungen

**Konfigurieren von Anwendungen**

1. [Schnellstart: Konfigurieren von Eigenschaften für eine Anwendung in Ihrem Azure Active Directory -Mandanten (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) zeigt Ihnen, wie Sie einige der Eigenschaften für eine App konfigurieren.
2. Um Ihre Anwendungen in Azure Active Directory zu integrieren, haben wir [eine Sammlung von Lernprogrammen](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) entwickelt, die Sie durch die Konfiguration führen.
3. [Wie Sie eine Anwendungsproxyanwendung konfigurieren,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) hilft Ihnen zu verstehen, wie Sie eine Anwendungsproxyanwendung innerhalb Azure AD konfigurieren, um Ihre lokalen Anwendungen für die Cloud verfügbar zu machen.
4. [Laden Sie PingAccess herunter, und konfigurieren Sie Ihre Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): Befolgen Sie die Anweisungen unter *Konfigurieren von PingAccess für Azure AD, um Anwendungen zu schützen*, die mit Microsoft Azure AD Anwendungsproxy auf der Ping Identity-Website veröffentlicht wurden, und laden Sie die neueste Version von PingAccess herunter.

**Fehler bei falsch konfigurierter Anwendung (AADSTS650056)**

1. Stellen Sie sicher, dass Sie über die vom Anwendungsbesitzer angegebene Anmeldeadresse auf die Anwendung zugreifen. Andernfalls müssen Sie sich über den normalen Prozess bei der Anwendung anmelden. In den meisten Fällen wird dies automatisch aufgelöst. Wenn dies nicht der Fall ist, kann dieser Beitrag bei der Problembehandlung und -behebung helfen.
2. **Wenn Ihre Organisation die Anwendung besitzt** (d. h. die Anwendungsregistrierung befindet sich in Ihrer Organisation):
    - Es wird empfohlen, dass mindestens die `User.Read` oder `openid` delegierte Berechtigung von **Microsoft Graph** hinzugefügt wird.
    - Stellen Sie sicher, dass die Anwendung und alle ihre Berechtigungen zustimmen. Sie können dies überprüfen, indem Sie sich die **Spalte "Status** " der Anwendungsregistrierung innerhalb von **API-Berechtigungen** ansehen.
    - In einigen Szenarien kann es sich bei der Anwendung um einen Drittanbieter handeln, aber sie kann in Ihrer Organisation registriert sein. Überprüfen Sie, ob diese Anwendung in Ihren App-Registrierungen aufgeführt ist (nicht Enterprise Anwendungen).
    - Wenn diese Fehlermeldung weiterhin angezeigt wird. Dann müssen Sie möglicherweise die in **Schritt 4** beschriebene Zustimmungs-URL erstellen.
3. **Wenn Ihre Organisation nicht der Anwendungsbesitzer ist und sie als Drittanbieteranwendung verwendet**:
    - Wenn Sie der globale/Unternehmensadministrator sind, sollte der Zustimmungsbildschirm angezeigt werden. Stellen Sie sicher, dass Sie das Kontrollkästchen **"Im Namen Ihrer Organisation zustimmen"** aktivieren.
    - Wenn der Zustimmungsbildschirm nicht angezeigt wird, löschen Sie die Enterprise Anwendung, und versuchen Sie es erneut.
    - Wenn diese Fehlermeldung weiterhin angezeigt wird. Dann müssen Sie möglicherweise die in **Schritt 4** beschriebene Zustimmungs-URL erstellen.
4. **Erstellen Sie manuell die zu verwendende Zustimmungs-URL**: Wenn die Anwendung für den Zugriff auf eine bestimmte Ressource konzipiert ist, können Sie möglicherweise nicht die Zustimmungsschaltflächen aus dem Azure-Portal verwenden. Sie müssen manuell Ihre eigene Zustimmungs-URL generieren und diese verwenden.
    - Sie müssen die `{App-Id}` und die `{App-Uri-Id}` vom Anwendungsbesitzer abrufen. `{Tenant-Id}` ist Ihr Mandantenbezeichner. Dies ist `yourdomain.onmicrosoft.com` entweder Ihre Verzeichnis-ID.
    - Wenn die Anwendung für die Ressource auf sich selbst zugreift, ist sie `{App-Id}` `{App-Uri-Id}` identisch.
5. Weitere Informationen finden Sie unter [Probleme beim Anmelden bei SAML-basierten, für einmaliges Anmelden konfigurierten Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Anpassen von Anwendungen**

- [Fügen Sie der Azure Active Directory Anmeldeseite Ihrer Organisation Branding](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) hinzu. Verwenden Sie das Logo Ihrer Organisation und benutzerdefinierte Farbschemas, um Ihren Azure Active Directory (Azure AD)-Anmeldeseiten ein einheitliches Aussehen und Verhalten zu verleihen.
- [Fügen Sie Ihren benutzerdefinierten Domänennamen über das Azure Active Directory-Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) hinzu . Jeder neue Azure AD Mandant enthält einen anfänglichen Domänennamen. Sie können den anfänglichen Domänennamen nicht ändern oder löschen, aber Sie können die Namen Ihrer Organisation hinzufügen. Das Hinzufügen von benutzerdefinierten Domänennamen hilft Ihnen beim Erstellen von Benutzernamen, die Ihren Benutzern vertraut sind.
