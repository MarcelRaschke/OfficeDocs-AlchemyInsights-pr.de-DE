---
title: Behandeln von Azure AD-Verknüpfungsproblemen
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
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939918"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Behandeln von Azure AD-Verknüpfungsproblemen

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die Einführung in die [Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) überprüft haben, die Sie darüber informieren, wie Sie Geräte unter die Kontrolle von Azure AD bringen. 
1. Wenn Sie Geräte direkt bei Azure AD registrieren und sie bei Intune registrieren, müssen Sie sicherstellen, dass Sie [Intune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) und die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) zuerst eingerichtet haben.
1. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.
1. Informationen zur Implementierung des Azure AD-Beitritts finden Sie unter Planen des [Azure AD-Beitritts.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Weitere Informationen zum Beheben allgemeiner Probleme beim Beitritt zu Azure AD finden Sie in den [häufig gestellten Fragen](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) zum Beitritt zu Azure Ad und zu Windows 10 Pro-Gerät finden Sie unter ["Nicht in der Lage, Windows 10 Pro Computer mit Azure AD zu verknüpfen – Upgrade auf – Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
