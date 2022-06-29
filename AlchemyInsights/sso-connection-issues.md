---
title: SSO-Verbindungsprobleme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 5de36838ba361d0f4b0c7c25dffc175969596cfc
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66417082"
---
# <a name="sso-connection-issues"></a>SSO-Verbindungsprobleme

1. Folgen Sie den Anweisungen unter [Schnellstart: Konfigurieren von Eigenschaften für eine Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) zum Konfigurieren Ihrer Anwendung.
2. Befolgen Sie je nach ausgewählter Option für Anwendung und [einmaliges Anmelden](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) die folgenden Anleitungen:
    - Informationen zum Konfigurieren einer **lokalen Anwendung** für **SAML-basiertes einmaliges Anmelden** finden Sie unter [SAML Single Sign-On für lokale Anwendungen mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Informationen zum Konfigurieren einer **Cloudanwendung** für **kennwortbasiertes einmaliges Anmelden** finden Sie unter  [Konfigurieren des einmaligen Anmeldens für Kennwörter](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Informationen zum Konfigurieren einer **lokalen Anwendung** für **einmaliges Anmelden über Anwendungsproxy** finden Sie unter [Kennworttresoring für einmaliges Anmelden mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Problembehandlung Anwendungsproxy Problemen**: Es wird empfohlen, mit der Überprüfung des Problembehandlungsflusses zu beginnen, [Anwendungsproxy Connector-Probleme zu debuggen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), um festzustellen, ob Anwendungsproxy Connectors ordnungsgemäß konfiguriert sind. Wenn sie weiterhin Probleme beim Herstellen einer Verbindung mit der Anwendung haben, folgen Sie dem Problembehandlungsfluss im [Debuggen Anwendungsproxy Anwendungsproblemen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Sie können [CORS-Probleme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) mithilfe von Browserdebuggingtools identifizieren:
    - Starten Sie den Browser, und navigieren Sie zu der Web-App.
    - Drücken Sie **F12**, um die Debuggingkonsole zu öffnen.
    - Versuchen Sie, die Transaktion zu reproduzieren, und überprüfen Sie die Konsolenmeldung. Eine CORS-Verletzung führt zu einem Konsolenfehler hinsichtlich des Ursprungs.
    - Einige CORS-Probleme können nicht behoben werden, z. B. wenn Ihre App zu login.microsoft.com zur Authentifizierung umleitet und das Zugriffstoken abläuft. Der CORS-Aufruf schlägt dann fehl. Eine Problemumgehung für dieses Szenario besteht im Verlängern der Gültigkeit des Zugriffstokens, um zu verhindern, dass es während einer Benutzersitzung abläuft. Weitere Informationen dazu finden Sie unter [Konfigurierbare Tokengültigkeitsdauer auf der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Problembehandlung bei SAML-basiertem einmaligem Anmelden**: Wir empfehlen, [Probleme bei der Anmeldung bei saml-basierten, für einmaliges Anmelden konfigurierten Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) zu überprüfen, um die Lösungen für die Probleme zu finden, auf die Sie am ehesten stoßen.
5. **Problembehandlung bei kennwortbasiertem einmaligem Anmelden**: Wir empfehlen, die [Problembehandlung für kennwortbasiertes einmaliges Anmelden in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) zu überprüfen, um die Lösungen für die Probleme zu finden, auf die Sie am ehesten stoßen.
6. Informationen zu Verbindungsproblemen bei der Verwendung eines VPN finden Sie unter [Verwenden von Single Sign On (SSO) über VPN und Wi-Fi Verbindungen](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
