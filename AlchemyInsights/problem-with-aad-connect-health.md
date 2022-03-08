---
title: Problem mit AAD Verbinden Integrität
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 1a96ea7d01a893eddbf9c74a2cfa37274bffe208
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63270665"
---
# <a name="problem-with-aad-connect-health"></a>Problem mit AAD Verbinden Integrität

- Stellen Sie sicher, dass Sie zum Ausführen des Vorgangs autorisiert sind. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die [rollenbasierte Zugriffssteuerung](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert sind und nicht aufgrund einer Firewall blockiert werden. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, da die ausgehende Kommunikation einer SSL-Überprüfung durch die Netzwerkschicht unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integrität überprüft haben. Überprüfen Sie Ihre Einstellung. In diesem [Leitfaden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) erfahren Sie, wie Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integritätsbenachrichtigungen konfigurieren.
- Weitere Informationen zum Synchronisierungsbericht AAD Verbinden Integrität und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Informationen zur Problembehandlung bei AAD Verbinden Integritätswarnungen finden Sie [im Handbuch zur Problembehandlung für AAD Verbinden Integritätsdaten-Aktualitätswarnungen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness). Häufig gestellte Fragen finden Sie unter [Allgemeine Fragen zur Installation AAD Verbinden Integrität](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
