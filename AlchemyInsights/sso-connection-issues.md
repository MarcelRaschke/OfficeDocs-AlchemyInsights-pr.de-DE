---
title: SSO-Verbindungsprobleme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 669c45e7c85f228f0c715668d1d42492e3097cc6
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62632290"
---
# <a name="sso-connection-issues"></a>SSO-Verbindungsprobleme

1. Folgen Sie den Anweisungen unter [Schnellstart: Konfigurieren von Eigenschaften für eine Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) zum Konfigurieren Ihrer Anwendung.
2. Folgen Sie je nach ausgewählter Anwendung und [Single Sign-On-Option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) den entsprechenden Anweisungen unten:
    - Informationen zum Konfigurieren einer **lokalen Anwendung** für **SAML-basiertes einmaliges Anmelden** finden Sie unter [SAML Single Sign-On für lokale Anwendungen mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Informationen zum Konfigurieren einer **Cloudanwendung** für **kennwortbasiertes einmaliges Anmelden** finden Sie unter  [Konfigurieren des einmaligen Kennworts](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Informationen zum Konfigurieren einer **lokalen Anwendung** für **einmaliges Anmelden über den Anwendungsproxy** finden Sie unter [Kennworttresor für einmaliges Anmelden mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Problembehandlung bei Anwendungsproxyproblemen**: Es wird empfohlen, mit der Überprüfung des Problembehandlungsflusses, [debuggen von Problemen mit anwendungsproxykonnektoren](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) zu beginnen, um festzustellen, ob Anwendungsproxyconnectors ordnungsgemäß konfiguriert sind. Wenn sie weiterhin Probleme beim Herstellen einer Verbindung mit der Anwendung haben, führen Sie den Problembehandlungsfluss unter [Debuggen von Anwendungsproxyanwendungsproblemen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) aus. Sie können [CORS-Probleme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) mithilfe von Browserdebuggertools identifizieren:
    - Starten Sie den Browser, und navigieren Sie zu der Web-App.
    - Drücken Sie **F12**, um die Debuggingkonsole zu öffnen.
    - Versuchen Sie, die Transaktion zu reproduzieren, und überprüfen Sie die Konsolenmeldung. Eine CORS-Verletzung führt zu einem Konsolenfehler hinsichtlich des Ursprungs.
    - Einige CORS-Probleme können nicht behoben werden, z. B. wenn Ihre App zur Authentifizierung zu login.microsoft.com umleitet und das Zugriffstoken abläuft. Der CORS-Aufruf schlägt dann fehl. Eine Problemumgehung für dieses Szenario besteht im Verlängern der Gültigkeit des Zugriffstokens, um zu verhindern, dass es während einer Benutzersitzung abläuft. Weitere Informationen dazu finden Sie unter [Konfigurierbare Tokengültigkeitsdauer auf der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Problembehandlung für SAML-basiertes einmaliges Anmelden**: Es wird empfohlen, [Probleme beim Anmelden bei SAML-basierten, für einmaliges Anmelden konfigurierten Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) zu überprüfen, um die Lösungen für die Probleme zu finden, auf die Sie am wahrscheinlichsten stoßen.
5. **Problembehandlung bei kennwortbasiertem einmaligem Anmelden**: Es wird empfohlen, die [Problembehandlung bei kennwortbasiertem einmaligem Anmelden in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) zu überprüfen, um lösungen für die Probleme zu finden, die am wahrscheinlichsten auftreten.
6. Informationen zu Verbindungsproblemen bei der Verwendung eines VPN finden Sie unter [Verwenden von einmaligem Anmelden (Single Sign On, SSO) über VPN und Wi-Fi Verbindungen](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
