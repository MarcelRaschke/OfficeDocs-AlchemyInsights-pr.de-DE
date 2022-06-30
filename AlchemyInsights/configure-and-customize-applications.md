---
title: Konfigurieren und Anpassen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: ab3f285e209f4c31c42f71ef1bef1ccf34fd4651
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66514884"
---
# <a name="configure-and-customize-applications"></a>Konfigurieren und Anpassen von Anwendungen

**Konfigurieren von Anwendungen**

1. [Schnellstart: Das Konfigurieren von Eigenschaften für eine Anwendung in Ihrem Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) zeigt Ihnen, wie Sie einige der Eigenschaften für eine App konfigurieren.
2. Um Ihre Anwendungen in Azure Active Directory zu integrieren, haben wir [eine Sammlung von Lernprogrammen](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) entwickelt, die Sie durch die Konfiguration führen.
3. [Wie Sie eine Anwendungsproxy-Anwendung konfigurieren](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to), hilft Ihnen zu verstehen, wie Sie eine Anwendungsproxy Anwendung in Azure AD konfigurieren, um Ihre lokalen Anwendungen in der Cloud verfügbar zu machen.
4. [Laden Sie PingAccess herunter, und konfigurieren Sie Ihre Anwendung](https://docs.pingidentity.com/bundle/pingaccess-43/page/agents/azure/pa_c_PAAzureSolutionOverview.html): Befolgen Sie die Anweisungen unter *Konfigurieren von PingAccess für Azure AD, um Anwendungen zu schützen*, die mithilfe von Microsoft Azure AD Anwendungsproxy auf der Ping Identity-Website veröffentlicht wurden, und laden Sie die neueste Version von PingAccess herunter.

**Fehler bei falsch konfigurierter Anwendung (AADSTS650056)**

1. Stellen Sie sicher, dass Sie über die vom Anwendungsbesitzer angegebene Anmeldeadresse auf die Anwendung zugreifen. Andernfalls bedeutet dies, dass Sie sich über den normalen Prozess bei der Anwendung anmelden. In den meisten Fällen wird dies automatisch aufgelöst. Wenn dies nicht der Tut, kann dieser Beitrag bei der Problembehandlung und -behebung helfen.
2. **Wenn Ihre Organisation der Besitzer der Anwendung** ist (d. h. die Anwendungsregistrierung befindet sich in Ihrer Organisation):
    - Mindestens wird empfohlen, dass die `User.Read` oder `openid` delegierte Berechtigung von **Microsoft Graph** hinzugefügt wird.
    - Stellen Sie sicher, dass der Anwendung und allen berechtigungen zugestimmt wird. Sie können dies überprüfen, indem Sie sich die Spalte **"Status** " der Anwendungsregistrierung in **API-Berechtigungen** ansehen.
    - In einigen Szenarien kann es sich bei der Anwendung um einen Drittanbieter handeln, sie ist jedoch möglicherweise in Ihrer Organisation registriert. Vergewissern Sie sich, dass diese Anwendung in Ihrem App-Registrierungen aufgeführt ist (keine Enterprise-Anwendungen).
    - Wenn diese Fehlermeldung weiterhin angezeigt wird. Anschließend müssen Sie möglicherweise die in **Schritt 4** beschriebene Zustimmungs-URL erstellen.
3. **Wenn Ihre Organisation nicht der Anwendungsbesitzer ist und sie als Drittanbieteranwendung verwendet**:
    - Wenn Sie der globale/Unternehmensadministrator sind, sollte der Zustimmungsbildschirm angezeigt werden. Stellen Sie sicher, dass Sie das Kontrollkästchen **"Zustimmung im Namen Ihrer Organisation"** aktivieren.
    - Wenn der Zustimmungsbildschirm nicht angezeigt wird, löschen Sie die Enterprise-Anwendung, und versuchen Sie es erneut.
    - Wenn diese Fehlermeldung weiterhin angezeigt wird. Anschließend müssen Sie möglicherweise die in **Schritt 4** beschriebene Zustimmungs-URL erstellen.
4. **Erstellen Sie die zu verwendende Zustimmungs-URL manuell**: Wenn die Anwendung für den Zugriff auf eine bestimmte Ressource konzipiert ist, können Sie möglicherweise die Schaltflächen "Zustimmung" der Azure-Portal nicht verwenden, müssen Sie ihre eigene Zustimmungs-URL manuell generieren und diese verwenden.
    - Sie müssen den und den `{App-Id}` `{App-Uri-Id}` vom Anwendungsbesitzer abrufen. `{Tenant-Id}` wird Ihr Mandantenbezeichner sein. Dies ist entweder `yourdomain.onmicrosoft.com` Ihre Verzeichnis-ID.
    - Wenn die Anwendung für die Ressource auf sich selbst zugreift, ist die `{App-Id}` `{App-Uri-Id}` Anwendung identisch.
5. Weitere Informationen finden Sie [unter Probleme bei der Anmeldung bei saml-basierten, für einmaliges Anmelden konfigurierten Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Anpassen von Anwendungen**

- [Hinzufügen von Branding zur Azure Active Directory-Anmeldeseite Ihrer Organisation](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – Verwenden Sie das Logo und benutzerdefinierte Farbschemas Ihrer Organisation, um Ein einheitliches Aussehen und Verhalten für Ihre Azure Active Directory (Azure AD)-Anmeldeseiten bereitzustellen.
- [Fügen Sie Ihren benutzerdefinierten Domänennamen mithilfe des Azure Active Directory-Portals](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) hinzu– Jeder neue Azure AD-Mandant verfügt über einen anfänglichen Domänennamen. Sie können den ursprünglichen Domänennamen nicht ändern oder löschen, aber Sie können die Namen Ihrer Organisation hinzufügen. Durch das Hinzufügen von benutzerdefinierten Domänennamen können Sie Benutzernamen erstellen, die Ihren Benutzern vertraut sind.
