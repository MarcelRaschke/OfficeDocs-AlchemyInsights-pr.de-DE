---
title: Behandeln von Problemen bei der Azure AD Hybrid-Einbindung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003244"
- "9003246"
- "6162"
- "6158"
ms.date: 08/06/2020
ms.openlocfilehash: 1638de38e05bae738d33dd5bb312d388bf1df5f3
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66261802"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Behandeln von Problemen bei der Azure AD Hybrid-Einbindung

Es wird dringend empfohlen, dass ein Gerät unter dem Systemkonto mithilfe des [Skripts zum Test der Geräteregistrierungskonnektivität](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) auf Endpunkte der Geräteregistrierung zugreifen kann.

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, lesen Sie unbedingt EI[nführung zur Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), um zu erfahren, wie Sie Azure AD die Steuerung von Geräten anvertrauen.
1. Wenn Sie Geräte direkt in Azure AD registrieren und für Intune registrieren, stellen Sie zuerst sicher, dass Sie [Intune konfiguriert haben](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) und die [-Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) zur Verfügung haben.
1. Stellen Sie sicher, dass Sie autorisiert sind, Vorgänge in Azure AD und lokalem AD durchzuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten. Wenn Sie außerdem automatische Registrierungen in Ihrem lokalen Active Directory einrichten, müssen Sie außerdem Administrator von Active Directory und (sofern zutreffend) AD FS sein.

Weitere Details zum Beheben potenzieller Probleme mit der Hybridverknüpfung finden Sie unter [Problembehandlung bei der Hybridverknüpfung](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) zum Einrichten von mit Azure AD verknüpften Hybridgeräten und zum Verwalten von Geräten mithilfe des Azure AD-Portals finden Sie unter [Einrichten von mit Azure AD verknüpften Hybridgeräten (lokal domänenverknüpften)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) und [Verwalten von Geräten mithilfe des Azure-Portals](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Informationen zum Beheben von häufig auftretenden Problemen bei der Azure AD Hybrid-Einbindung finden Sie unter [Häufig gestellte Fragen zu Azure AD Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
