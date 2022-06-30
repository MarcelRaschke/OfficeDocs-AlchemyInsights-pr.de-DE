---
title: Probleme bei der Integration nahtloser SSO in meine lokalen Apps
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004356"
- "7798"
ms.date: 01/13/2021
ms.openlocfilehash: 1e0d90cf4964f4acb42b3766ab675389d4902f1d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66433903"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Probleme bei der Integration nahtloser SSO in meine lokalen Apps

Gehen Sie wie folgt vor, um Probleme mit der Integration nahtloser SSO in lokale Anwendungen zu beheben:

**Empfohlene Schritte**

1. Informationen zum Konfigurieren einer **lokalen Anwendung** für **einmaliges Anmelden über Anwendungsproxy** finden Sie unter [Kennworttresoring für einmaliges Anmelden mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Problembehandlung bei Anwendungsproxy Problemen**: Es wird empfohlen, mit der Überprüfung des Problembehandlungsablaufs zu beginnen, [Anwendungsproxy Connector-Probleme zu debuggen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), um festzustellen, ob Anwendungsproxy Connectors ordnungsgemäß konfiguriert sind. Wenn weiterhin Probleme beim Herstellen einer Verbindung mit der Anwendung bestehen, führen Sie die Schritte zur Problembehandlung unter [Debuggen von Problemen mit Anwendungsproxyanwendungen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) aus. Sie können [CORS-Probleme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) mithilfe der folgenden Browserdebuggingtools identifizieren:
    1. Starten Sie den Browser, und navigieren Sie zu der Web-App.
    1. Drücken Sie **F12**, um die Debuggingkonsole zu öffnen.
    1. Versuchen Sie, die Transaktion zu reproduzieren, und überprüfen Sie die Konsolenmeldung. Eine CORS-Verletzung führt zu einem Konsolenfehler hinsichtlich des Ursprungs.
    1. Einige CORS-Probleme können nicht behoben werden, z. B. wenn Ihre App zu login.microsoftonline.com umleitet, um sich zu authentifizieren, und das Zugriffstoken abläuft. Der CORS-Aufruf schlägt dann fehl. Eine Problemumgehung für dieses Szenario besteht im Verlängern der Gültigkeit des Zugriffstokens, um zu verhindern, dass es während einer Benutzersitzung abläuft. Weitere Informationen dazu finden Sie unter [Konfigurierbare Tokengültigkeitsdauer auf der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Empfohlene Dokumente**

- [Konfigurieren des einmaligen Anmeldens bei einer Anwendungsproxy-Anwendung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML-Einmaliges Anmelden für lokale Anwendungen mit Anwendungsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Grundlegendes und Lösen von Azure Active Directory Anwendungsproxy CORS-Problemen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Problembehandlung bei eingeschränkten Kerberos-Delegierungskonfigurationen für Anwendungsproxys](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)