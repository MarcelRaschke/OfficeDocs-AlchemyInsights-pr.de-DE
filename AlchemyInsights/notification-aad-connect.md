---
title: Benachrichtigung AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: feafeefe734d378f03ab1c5d207e36de838bec33
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66350463"
---
# <a name="notification-aad-connect"></a>Benachrichtigung AAD Connect

- Stellen Sie sicher, dass Sie berechtigt sind, den Vorgang auszuführen. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie [rollenbasierte Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert und nicht aufgrund der Firewall blockiert sind. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, weil die ausgehende Kommunikation von der Netzwerkschicht einer SSL-Überprüfung unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Connect Health überprüft haben, und überprüfen Sie Ihre Einstellung. Informationen zum Konfigurieren der Benachrichtigungseinstellungen für Azure AD Connect-Integritätsbenachrichtigungen finden Sie in diesem [Handbuch](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Weitere Informationen zum AAD Connect-Integritätssynchronisierungsbericht und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Informationen zur Problembehandlung bei AAD Connect-Integritätswarnungen finden Sie im [Handbuch zur Problembehandlung für AAD Connect Integritätsdaten-Aktualitätswarnungen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) und für häufig gestellte Fragen unter [Allgemeinen Fragen zur AAD Connect-Integritätsinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
