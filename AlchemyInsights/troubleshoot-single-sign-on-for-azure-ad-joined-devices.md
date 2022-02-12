---
title: Problembehandlung beim einmaligen Anmelden für Azure AD eingebundene Geräte
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
ms.openlocfilehash: 87a3b5d6ae573fb38d831253fb4ce0cc23475eba
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62596270"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Problembehandlung beim einmaligen Anmelden für Azure AD eingebundene Geräte

Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre in die AD-Domäne eingebundenen Computer mit Azure AD verknüpfen möchten, können Sie dies durch hybride Azure AD Verknüpfung erreichen. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

Weitere Informationen finden Sie unter [Konfigurieren Azure AD verbundener Geräte für lokale Single-Sign On mithilfe von Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Probleme mit dem primären Aktualisierungstoken (PRT)**

Ein primäres Aktualisierungstoken (PRT) ist ein Schlüsselartefakt der Azure AD Authentifizierung auf Windows 10, Windows Server 2016 und neueren Versionen, iOS- und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Erstanbietern von Microsoft ausgestellt wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die auf diesen Geräten verwendeten Anwendungen zu aktivieren. Ausführliche Informationen dazu, wie ein PRT auf Windows 10 Geräten ausgestellt, verwendet und geschützt wird, finden Sie unter [Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES und AzureADPrt: JA**

Diese Felder geben an, ob sich der Benutzer bei der Anmeldung am Gerät erfolgreich bei Azure AD authentifiziert hat. Wenn die Werte **"NO**" lauten, kann dies folgende Ursachen haben:

- Ungültiger Speicherschlüssel im TPM, der dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie keySignTest, während Sie erhöhte Rechte ausführen).
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Informationen zur Problembehandlung für Geräte mithilfe des Befehls "dsregcmd" finden Sie unter [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
