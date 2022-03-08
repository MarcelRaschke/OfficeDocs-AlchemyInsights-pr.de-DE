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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 82d2897502220e585b078156deee4c9ae7695b7a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63198752"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Einmaliges Anmelden für Azure Active Directory verbundene Geräte

Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre in die AD-Domäne eingebundenen Computer mit Azure AD verknüpfen möchten, können Sie dies durch hybride Azure AD Verknüpfung erreichen. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Konfigurieren Azure AD verbundener Geräte für lokale Single-Sign On mit Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Probleme mit dem primären Aktualisierungstoken (PRT)** Ein primäres Aktualisierungstoken (PRT) ist ein Schlüsselartefakt der Azure AD Authentifizierung auf Windows 10, Windows Server 2016 und neueren Versionen, iOS- und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Erstanbietern von Microsoft ausgestellt wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die auf diesen Geräten verwendeten Anwendungen zu aktivieren. [Unter "Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)" geben wir Details dazu an, wie ein PRT auf Windows 10 Geräten ausgestellt, verwendet und geschützt wird.

**WamDefaultSet: YES und AzureADPrt: JA** Diese Felder geben an, ob der Benutzer bei der Anmeldung am Gerät erfolgreich bei Azure AD authentifiziert wurde. Wenn die Werte **"NO**" lauten, kann folgendes fällig sein:

- Ungültiger Speicherschlüssel im TPM, der dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie keySignTest, während Sie mit erhöhten Rechten ausgeführt werden).
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Problembehandlung bei Geräten mithilfe des Befehls "dsregcmd" – [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
