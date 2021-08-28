---
title: Single-Sign für Azure Active Directory verbundene Geräte aktiviert
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
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050009"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Einmaliges Anmelden für Azure Active Directory verbundene Geräte

Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre mit der AD-Domäne verbundenen Computer mit Azure AD verknüpfen möchten, können Sie dies erreichen, indem Sie eine Azure AD-Hybridverknüpfung durchführen. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Konfigurieren von in Azure AD eingebundenen Geräten für lokale Single-Sign On mithilfe von Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Probleme mit dem primären Aktualisierungstoken (PRT)** Ein primäres Aktualisierungstoken (PRT) ist ein Schlüsselartefakt der Azure AD-Authentifizierung auf Windows 10, Windows Server 2016 und neueren Versionen, iOS- und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Erstanbietern von Microsoft ausgestellt wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die auf diesen Geräten verwendeten Anwendungen zu aktivieren. [Unter "Was ist ein primäres Aktualisierungstoken?"](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)werden Details dazu bereitgestellt, wie ein PRT auf Windows 10 Geräten ausgestellt, verwendet und geschützt wird.

**WamDefaultSet: YES und AzureADPrt: JA** Diese Felder geben an, ob der Benutzer sich bei Azure AD bei der Anmeldung am Gerät erfolgreich authentifiziert hat. Wenn die Werte **"NO"** lauten, kann folgendes fällig sein:

- Ungültiger Speicherschlüssel im TPM, der dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie keySignTest, während Sie erhöhte Rechte ausführen).
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Problembehandlung bei Geräten mithilfe des Befehls "dsregcmd" – [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
