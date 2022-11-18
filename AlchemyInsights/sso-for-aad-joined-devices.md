---
title: Single-Sign für in Azure Active Directory eingebundene Geräte aktiviert
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003257"
- "9891"
ms.date: 03/24/2021
ms.openlocfilehash: 3d63a1d45724bf8a88dea45abc7fc3a249a5d63b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66262702"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Einmaliges Anmelden für in Azure Active Directory eingebundene Geräte

Wenn Sie über eine lokales Active Directory (AD)-Umgebung verfügen und Ihre in die AD-Domäne eingebundenen Computer mit Azure AD verknüpfen möchten, können Sie dies mithilfe einer Hybrid-Azure AD-Verknüpfung erreichen. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Konfigurieren von in Azure AD eingebundenen Geräten für lokale Single-Sign On mithilfe von Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Probleme mit dem primären Aktualisierungstoken (PRT)** Ein primäres Aktualisierungstoken (PRT) ist ein wichtiges Artefakt der Azure AD-Authentifizierung auf Windows 10, Windows Server 2016 und höheren Versionen, iOS und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell an Microsoft-Tokenbroker von Erstanbietern ausgestellt wurde, um einmaliges Anmelden (Single Sign-On, SSO) in allen Anwendungen zu aktivieren, die auf diesen Geräten verwendet werden. [In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.

**WamDefaultSet: YES und AzureADPrt: YES** Diese Felder geben an, ob sich der Benutzer bei der Anmeldung beim Gerät erfolgreich bei Azure AD authentifiziert hat. Wenn die Werte **NEIN** sind, kann dies fällig sein:

- Ungültiger Speicherschlüssel im TPM, das dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie keysigntest, während Sie mit erhöhten Rechten ausgeführt werden).
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Problembehandlung bei Geräten mit dem Befehl "dsregcmd" – [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
