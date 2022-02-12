---
title: Problem mit AAD Verbinden Integrität
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
- "9004649"
- "8427"
ms.openlocfilehash: 4b09686d3484c404664ac86ca23a6978119d56a7
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62648112"
---
# <a name="problem-with-aad-connect-health"></a>Problem mit AAD Verbinden Integrität

- Stellen Sie sicher, dass Sie zum Ausführen des Vorgangs autorisiert sind. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die [rollenbasierte Zugriffssteuerung](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert sind und nicht aufgrund einer Firewall blockiert werden. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, da die ausgehende Kommunikation einer SSL-Überprüfung durch die Netzwerkschicht unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integrität überprüft haben. Überprüfen Sie Ihre Einstellung. In diesem [Leitfaden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) erfahren Sie, wie Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integritätsbenachrichtigungen konfigurieren.
- Weitere Informationen zum Synchronisierungsbericht AAD Verbinden Integrität und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Informationen zur Problembehandlung bei AAD Verbinden Integritätswarnungen finden Sie [im Handbuch zur Problembehandlung für warnungen zur Aktualität von AAD Verbinden Integritätsdaten](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness). Häufig gestellte Fragen zur Installation von Integritätsinformationen finden Sie unter [Common AAD Verbinden Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
