---
title: Problembehandlung bei Azure AD Verknüpfungsproblemen
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
ms.openlocfilehash: 23b6843150123e333a220497b6581a7971837722
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63220893"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Problembehandlung bei Azure AD Verknüpfungsproblemen

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die [Einführung in die Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) überprüft haben, die Sie darüber informieren, wie Sie Geräte unter die Kontrolle Azure AD. 
1. Wenn Sie Geräte direkt bei Azure AD registrieren und sie bei Intune registrieren, müssen Sie sicherstellen, dass Sie [Intune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) und die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) zuerst eingerichtet haben.
1. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.
1. Informationen zu Azure AD Implementierung des Beitritts finden Sie unter [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Weitere Informationen zum Beheben häufiger Probleme mit Azure AD Beitritt finden Sie in den [häufig gestellten Fragen zum Beitritt zu Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) und für Windows 10 Pro-Gerät unter ["Nicht in der Lage, Windows 10 Pro Computer mit Azure AD zu verknüpfen – Upgrade auf " Microsoft Community](https://answers.microsoft.com/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
