---
title: Benachrichtigungs-AAD Verbinden
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
- "9003245"
- "9326"
ms.openlocfilehash: 7e690ef4a9ae8e7f3319ced44fe12f60f84b8a10
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62648841"
---
# <a name="notification-aad-connect"></a>Benachrichtigungs-AAD Verbinden

- Stellen Sie sicher, dass Sie zum Ausführen des Vorgangs autorisiert sind. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die [rollenbasierte Zugriffssteuerung](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert sind und nicht aufgrund einer Firewall blockiert werden. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, da die ausgehende Kommunikation einer SSL-Überprüfung durch die Netzwerkschicht unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integrität überprüft haben, und überprüfen Sie Ihre Einstellung. Informationen zum Konfigurieren der Benachrichtigungseinstellungen für Azure AD Verbinden Integritätsbenachrichtigungen finden Sie in diesem [Leitfaden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Weitere Informationen zum Synchronisierungsbericht AAD Verbinden Integrität und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Informationen zur Problembehandlung bei AAD Verbinden Integritätswarnungen finden Sie [im Handbuch zur Problembehandlung für Warnungen zur Aktualität von Integritätsdaten AAD Verbinden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) und häufig gestellte Fragen finden Sie unter [allgemeine Fragen zur Installation AAD Verbinden Integrität](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
