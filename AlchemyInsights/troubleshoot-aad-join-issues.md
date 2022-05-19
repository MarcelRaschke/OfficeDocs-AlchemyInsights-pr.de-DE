---
title: Behandeln von Azure AD-Beitrittsproblemen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 6b3a9fa97dc93d6689ba5f71aa2c8a98a4d1a8a8
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65592030"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Behandeln von Azure AD-Beitrittsproblemen

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die [Einführung in die Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) überprüft haben, die Sie dazu führt, wie Sie Geräte unter die Kontrolle von Azure AD bringen. 
1. Wenn Sie Geräte direkt bei Azure AD registrieren und bei Intune registrieren, müssen Sie sicherstellen, dass Sie [Intune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) haben und zuerst über die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) verfügen.
1. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.
1. Informationen zur Azure AD-Beitrittsimplementierung finden Sie unter [Planen des Azure AD-Beitritts](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Weitere Informationen zum Beheben häufiger Probleme mit der Azure AD-Teilnahme finden [Sie unter Häufig gestellte Fragen zum Azure Ad-Beitritt](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) und für Windows 10 Pro-Gerät unter ["Nicht in der Lage, Windows 10 Pro Computer zu Azure AD zu verbinden – Upgrade erforderlich – Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/all/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
