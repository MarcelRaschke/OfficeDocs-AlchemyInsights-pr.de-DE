---
title: AAD-Verbinden für Benachrichtigungen
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
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097305"
---
# <a name="notification-aad-connect"></a>AAD-Verbinden für Benachrichtigungen

- Stellen Sie sicher, dass Sie zum Ausführen des Vorgangs autorisiert sind. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die [rollenbasierte Zugriffssteuerung](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) verwenden, um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert sind und nicht aufgrund einer Firewall blockiert werden. Ausführliche Informationen finden Sie unter ["Anforderungen".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Die Registrierung kann fehlschlagen, da die ausgehende Kommunikation einer SSL-Überprüfung durch die Netzwerkschicht unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Verbinden Integrität überprüft haben, und überprüfen Sie Ihre Einstellung. Informationen zum Konfigurieren der Benachrichtigungseinstellungen für Azure AD Verbinden Integritätsbenachrichtigungen finden Sie in diesem [Leitfaden.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Weitere Informationen zum AAD-Verbinden Integritätssynchronisierungsbericht und zum Herunterladen finden Sie im [Synchronisierungsbericht auf Objektebene.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Informationen zur Problembehandlung bei AAD Verbinden Integritätswarnungen finden Sie [im Handbuch zur Problembehandlung für AAD Verbinden Integritätsdaten-Aktualitätswarnungen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) und häufig gestellte Fragen finden Sie unter [Allgemeine Fragen zur Installation von AAD Verbinden Integrität.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
