---
title: Problembehandlung beim einmaligen Anmelden für in Azure AD eingebundene Geräte
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 5c58235c3d671fe105dccbf264406382eefc4300
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66333932"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Problembehandlung beim einmaligen Anmelden für in Azure AD eingebundene Geräte

Wenn Sie über eine lokales Active Directory (AD)-Umgebung verfügen und Ihre in die AD-Domäne eingebundenen Computer mit Azure AD verknüpfen möchten, können Sie dies mithilfe einer Hybrid-Azure AD-Verknüpfung erreichen. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

Weitere Informationen finden Sie unter [Konfigurieren von in Azure AD eingebundenen Geräten für lokale Single-Sign On mithilfe von Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Probleme mit dem primären Aktualisierungstoken (PRT)**

Ein primäres Aktualisierungstoken (PRT) ist ein wichtiges Artefakt der Azure AD-Authentifizierung auf Windows 10, Windows Server 2016 und höheren Versionen, iOS und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell an Microsoft-Tokenbroker von Erstanbietern ausgestellt wurde, um einmaliges Anmelden (Single Sign-On, SSO) in allen Anwendungen zu aktivieren, die auf diesen Geräten verwendet werden. Ausführliche Informationen dazu, wie ein PRT auf Windows 10 Geräten ausgestellt, verwendet und geschützt wird, finden Sie unter [Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES und AzureADPrt: YES**

Diese Felder geben an, ob sich der Benutzer bei der Anmeldung beim Gerät erfolgreich bei Azure AD authentifiziert hat. Wenn die Werte **NEIN** sind, kann dies folgende Ursachen haben:

- Ungültiger Speicherschlüssel im TPM, das dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie keysigntest, während Sie mit erhöhten Rechten ausgeführt werden)
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Informationen zur Problembehandlung für Geräte mit dem Befehl "dsregcmd" finden Sie unter ["SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)".
