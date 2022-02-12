---
title: Kennwortsynchronisierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 8ae1e497aa92f81a0d365e936644c3e61628df36
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62634342"
---
# <a name="password-synchronization"></a>Kennwortsynchronisierung

**Kennworthashsynchronisierung funktioniert überhaupt nicht**

Einige häufige Probleme, die Kunden auftreten, wenn die Kennworthashsynchronisierung nicht funktioniert, sind:

- Dem Active Directory-Konto, das von Azure AD Verbinden für die Kommunikation mit lokalem Active Directory verwendet wird, wird nicht die Berechtigung "**Verzeichnisänderungen replizieren**" und "**Verzeichnisänderungen replizieren"** gewährt, die für die Kennwortsynchronisierung erforderlich sind. Sie müssen dies beheben, indem Sie diese Berechtigungen dem Active Directory-Konto erteilen.
- Die Kennworthashsynchronisierung ist deaktiviert, nachdem ein Administrator die User Sign-In-Methode von der **Kennwortsynchronisierung** in eine andere Option geändert hat, z **. B. partnerverbunden mit AD FS** im Assistenten Azure AD Verbinden . Sie können dies beheben, indem Sie das **Kennworthashsynchronisierungsfeature** im Assistenten Azure AD Verbinden erneut aktivieren.
- Konnektivitätsproblem mit lokalem Active Directory. Beispielsweise können Azure AD Verbinden nicht auf einige Domänencontroller zugreifen, oder die [erforderlichen Ports](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) werden von der Firewall blockiert. Sie müssen dies beheben, indem Sie sicherstellen, dass die Verbindung zwischen dem Azure AD Verbinden-Server und dem lokalen Active Directory ordnungsgemäß funktioniert.
- Azure AD Verbinden Server, der sich derzeit im Stagingmodus befindet, was dazu führt, dass der Server nicht in der Lage ist, die Kennworthashes zu verwenden. Um das Problem zu beheben, führen Sie die im Abschnitt ["Problembehandlung bei der Kennwortsynchronisierung mit Azure AD Verbinden Synchronisierung" beschriebenen Schritte aus . Es werden keine Kennwörter synchronisiert](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Kennworthashsynchronisierung funktioniert für einige meiner Benutzer nicht**

1. Wenn Sie bemerkt haben, dass der Kennworthash für einen Benutzer nicht synchronisiert wird, verwenden Sie die **Problembehandlungsaufgabe** im Azure AD Verbinden, um das Problem zu untersuchen und zu beheben. Führen Sie die folgenden Aufgaben aus:

    a. [Ausführen der Problembehandlungsaufgabe im Assistenten](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Verwenden des Cmdlets zur Problembehandlung, um das Problem bei der Kennworthashsynchronisierung für eine bestimmte Verwendung zu untersuchen](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Das lokale Active Directory-Benutzerobjekt ist für Benutzer aktiviert und **muss bei der nächsten Anmeldeoption das Kennwort ändern** . Wenn diese Option aktiviert ist, wird dem Benutzer ein temporäres Kennwort zugewiesen, und er wird aufgefordert, das Kennwort bei der nächsten Anmeldung zu ändern. Azure AD Verbinden synchronisiert temporäre Kennwörter nicht mit Azure AD.

Führen Sie eine der folgenden Aufgaben aus, um das oben beschriebene Problem zu beheben:

- Bitten Sie den Benutzer, sich bei der lokalen Anwendung (z. B. Windows Desktop) anzumelden und das Kennwort zu ändern. Das neue Kennwort wird mit Azure AD synchronisiert.
- Lassen Sie einen Administrator das Kennwort des Benutzers aktualisieren, ohne die Option zu aktivieren, **muss der Benutzer bei der nächsten Anmeldung das Kennwort ändern** und das neue Kennwort für den Benutzer freigeben.

3. Das lokale Active Directory-Benutzerobjekt ist **nicht ordnungsgemäß** für die Objektsynchronisierung oder Kennwortsynchronisierung konfiguriert. Um dieses Problem zu beheben, führen Sie die in der [Problembehandlung für die Kennworthashsynchronisierung mit Azure AD Verbinden Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization) beschriebenen Schritte aus.







