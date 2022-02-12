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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: a694c471fe67838b459dc8b0784785c2c22127af
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62742599"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Problembehandlung bei Azure AD Verknüpfungsproblemen

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie "[Einführung in die Geräteverwaltung" in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) überprüft haben, die Sie darüber informieren, wie Sie Geräte unter die Kontrolle Azure AD. 
1. Wenn Sie Geräte direkt bei Azure AD registrieren und sie bei Intune registrieren, müssen Sie sicherstellen, dass Sie [Intune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) und die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) zuerst eingerichtet haben.
1. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.
1. Informationen zu Azure AD Implementierung des Beitritts finden Sie unter [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Weitere Informationen zum Beheben häufiger Probleme mit Azure AD Beitritt finden Sie in den [häufig gestellten Fragen zum Beitritt zu Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) und für Windows 10 Pro-Gerät unter ["Nicht in der Lage, Windows 10 Pro Computer mit Azure AD zu verknüpfen – Upgrade auf " Microsoft Community](https://answers.microsoft.com/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
