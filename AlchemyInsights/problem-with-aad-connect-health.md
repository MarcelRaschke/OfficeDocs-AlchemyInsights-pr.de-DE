---
title: Problem mit AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: eb9b313110e2204e654f4f351863b40d1400a920
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66292798"
---
# <a name="problem-with-aad-connect-health"></a>Problem mit AAD Connect Health

- Stellen Sie sicher, dass Sie berechtigt sind, den Vorgang auszuführen. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie [rollenbasierte Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert und nicht aufgrund der Firewall blockiert sind. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, weil die ausgehende Kommunikation von der Netzwerkschicht einer SSL-Überprüfung unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Connect Health überprüft haben. Bitte überprüfen Sie Ihre Einstellung. Dieses [Handbuch](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) hilft Ihnen zu verstehen, wie Sie die Benachrichtigungseinstellungen für Azure AD Connect-Integritätsbenachrichtigungen konfigurieren.
- Weitere Informationen zum AAD Connect-Integritätssynchronisierungsbericht und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Um Probleme mit AAD Connect-Integritätswarnungen zu beheben, folgen Sie [dem Problembehandlungshandbuch für AAD Connect Integritätsdaten-Aktualitätswarnungen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) und für häufig gestellte Fragen, siehe [allgemeine Fragen zur AAD Connect-Integritätsinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
