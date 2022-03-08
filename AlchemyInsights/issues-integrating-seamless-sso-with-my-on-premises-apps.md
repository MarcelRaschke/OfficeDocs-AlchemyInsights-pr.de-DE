---
title: Probleme bei der Integration von nahtlosen SSO in meine lokalen Apps
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: e8cd50222324f7cca9fa817bcb61702d513708c1
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63246329"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Probleme bei der Integration von nahtlosen SSO in meine lokalen Apps

Führen Sie die folgenden Schritte aus, um Probleme bei der Integration von nahtlosen SSO in lokale Anwendungen zu beheben:

**Empfohlene Schritte**

1. Informationen zum Konfigurieren einer **lokalen Anwendung** für **einmaliges Anmelden über den Anwendungsproxy** finden Sie unter [Kennworttresor für einmaliges Anmelden mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Problembehandlung bei Anwendungsproxyproblemen**: Es wird empfohlen, mit der Überprüfung des Problembehandlungsflusses, [dem Debuggen von Problemen mit anwendungsproxykonnektoren](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) zu beginnen, um festzustellen, ob Anwendungsproxyconnectors ordnungsgemäß konfiguriert sind. Wenn weiterhin Probleme beim Herstellen einer Verbindung mit der Anwendung bestehen, führen Sie die Schritte zur Problembehandlung unter [Debuggen von Problemen mit Anwendungsproxyanwendungen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) aus. Sie können [CORS-Probleme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) mithilfe der folgenden Browserdebuggertools identifizieren:
    1. Starten Sie den Browser, und navigieren Sie zu der Web-App.
    1. Drücken Sie **F12**, um die Debuggingkonsole zu öffnen.
    1. Versuchen Sie, die Transaktion zu reproduzieren, und überprüfen Sie die Konsolenmeldung. Eine CORS-Verletzung führt zu einem Konsolenfehler hinsichtlich des Ursprungs.
    1. Einige CORS-Probleme können nicht behoben werden, z. B. wenn Ihre App zur Authentifizierung zu login.microsoftonline.com umleitet und das Zugriffstoken abläuft. Der CORS-Aufruf schlägt dann fehl. Eine Problemumgehung für dieses Szenario besteht im Verlängern der Gültigkeit des Zugriffstokens, um zu verhindern, dass es während einer Benutzersitzung abläuft. Weitere Informationen dazu finden Sie unter [Konfigurierbare Tokengültigkeitsdauer auf der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Empfohlene Dokumente**

- [Konfigurieren des einmaligen Anmeldens bei einer Anwendungsproxyanwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML Single Sign-On für lokale Anwendungen mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Verstehen und Lösen Azure Active Directory Anwendungsproxy-CORS-Probleme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Problembehandlung bei eingeschränkten Kerberos-Delegierungskonfigurationen für Anwendungsproxys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)