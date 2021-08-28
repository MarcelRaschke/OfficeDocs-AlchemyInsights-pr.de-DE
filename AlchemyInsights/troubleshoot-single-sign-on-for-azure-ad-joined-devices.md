---
title: Problembehandlung bei single-sign-on für Azure AD-geräte
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039245"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Problembehandlung bei single-sign-on für Azure AD-geräte

Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre mit der AD-Domäne verbundenen Computer mit Azure AD verknüpfen möchten, können Sie dies erreichen, indem Sie eine Azure AD-Hybridverknüpfung durchführen. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

Weitere Informationen finden Sie unter [Konfigurieren von in Azure AD eingebundenen Geräten für lokale Single-Sign On mit Windows Hello for Business.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Probleme mit dem primären Aktualisierungstoken (PRT)**

Ein primäres Aktualisierungstoken (PRT) ist ein Schlüsselartefakt der Azure AD-Authentifizierung auf Windows 10, Windows Server 2016 und neueren Versionen, iOS- und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Erstanbietern von Microsoft ausgestellt wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die auf diesen Geräten verwendeten Anwendungen zu aktivieren. Ausführliche Informationen dazu, wie ein PRT auf Windows 10 Geräten ausgestellt, verwendet und geschützt wird, finden Sie unter [Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES und AzureADPrt: JA**

Diese Felder geben an, ob der Benutzer sich bei Azure AD bei der Anmeldung am Gerät erfolgreich authentifiziert hat. Wenn die Werte **NEIN** sind, kann dies auf Folgendes zurückzuführen sein:

- Ungültiger Speicherschlüssel im TPM, der dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie keySignTest, während Sie erhöhte Rechte ausführen).
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Informationen zur Problembehandlung von Geräten mit dem Befehl "dsregcmd" finden Sie unter [SSO-Status.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
