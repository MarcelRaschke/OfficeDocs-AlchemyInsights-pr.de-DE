---
title: Problem mit AAD Verbinden Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923751"
---
# <a name="problem-with-aad-connect-health"></a>Problem mit AAD Verbinden Health

- Stellen Sie sicher, dass Sie zum Ausführen des Vorgangs autorisiert sind. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die [rollenbasierte Zugriffssteuerung](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert sind und nicht aufgrund einer Firewall blockiert werden. Ausführliche Informationen finden Sie unter ["Anforderungen".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Die Registrierung kann fehlschlagen, da die ausgehende Kommunikation einer SSL-Überprüfung durch die Netzwerkschicht unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Health überprüft haben. Überprüfen Sie Ihre Einstellung. In diesem [Leitfaden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) erfahren Sie, wie Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integritätsbenachrichtigungen konfigurieren.
- Weitere Informationen zum AAD-Verbinden Integritätssynchronisierungsbericht und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Informationen zur Problembehandlung bei AAD Verbinden Integritätswarnungen finden Sie [im Handbuch zur Problembehandlung für AAD Verbinden Integritätsdaten-Aktualitätswarnungen.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Häufig gestellte Fragen finden Sie unter [Common AAD Verbinden Health installation questions.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
