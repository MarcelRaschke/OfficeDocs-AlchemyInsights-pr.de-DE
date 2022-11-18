---
title: Kennwortsynchronisierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004595"
- "8619"
ms.date: 02/24/2021
ms.openlocfilehash: 7a1623abf58b12657e1569619eefc668ec8487b1
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66386985"
---
# <a name="password-synchronization"></a>Kennwortsynchronisierung

**Kennworthashsynchronisierung funktioniert überhaupt nicht**

Einige häufige Probleme, die bei Kunden auftreten, wenn die Kennworthashsynchronisierung nicht funktioniert, sind:

- Das Active Directory-Konto, das von Azure AD Connect für die Kommunikation mit lokales Active Directory verwendet wird, erhält keine Berechtigungen zum **Replizieren von Verzeichnisänderungen** und **Replizieren von Verzeichnisänderungen Alle** Berechtigungen, die für die Kennwortsynchronisierung erforderlich sind. Sie müssen dies beheben, indem Sie dem Active Directory-Konto diese Berechtigungen erteilen.
- Die Kennworthashsynchronisierung wird deaktiviert, nachdem ein Administrator die Methode "Benutzer Sign-In" von " **Kennwortsynchronisierung** " in eine andere Option wie " **Verbund mit AD FS** " im Azure AD Connect-Assistenten geändert hat. Sie können dies beheben, indem Sie das Feature für die **Kennworthashsynchronisierung** im Azure AD Connect-Assistenten erneut aktivieren.
- Verbindungsproblem mit lokales Active Directory. Auf einige Domänencontroller kann z. B. von Azure AD Connect nicht zugegriffen werden, oder die [erforderlichen Ports](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) werden von der Firewall blockiert. Sie müssen dies beheben, indem Sie sicherstellen, dass die Konnektivität zwischen dem Azure AD Connect-Server und dem lokales Active Directory ordnungsgemäß funktioniert.
- Azure AD Connect-Server befindet sich derzeit im Stagingmodus, was dazu führt, dass der Server die Kennworthashes nicht abrufen kann. Führen Sie zur Problembehandlung die im Abschnitt ["Problembehandlung bei der Kennwortsynchronisierung mit Azure AD Connect-Synchronisierung" beschriebenen Schritte aus – es werden keine Kennwörter synchronisiert](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Die Kennworthashsynchronisierung funktioniert für einige meiner Benutzer nicht**

1. Wenn Sie bemerkt haben, dass der Kennworthash für einen Benutzer nicht synchronisiert wird, verwenden Sie die **Problembehandlungsaufgabe** in Azure AD Connect, um das Problem zu untersuchen und zu beheben. Führen Sie die folgenden Aufgaben aus:

    a. [Ausführen der Problembehandlungsaufgabe im Assistenten](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Verwenden Des Problembehandlungs-Cmdlets, um das Problem der Kennworthashsynchronisierung für eine bestimmte Verwendung zu untersuchen](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Das lokales Active Directory Benutzerobjekt ist aktiviert, damit **der Benutzer das Kennwort bei der nächsten Anmeldeoption ändern muss**. Wenn diese Option aktiviert ist, wird dem Benutzer ein temporäres Kennwort zugewiesen und bei der nächsten Anmeldung aufgefordert, das Kennwort zu ändern. Azure AD Connect synchronisiert keine temporären Kennwörter mit Azure AD.

Führen Sie eine der folgenden Aufgaben aus, um das oben genannte Problem zu beheben:

- Bitten Sie den Benutzer, sich bei der lokalen Anwendung (z. B. Windows Desktop) anzumelden und das Kennwort zu ändern. Das neue Kennwort wird mit Azure AD synchronisiert.
- Lassen Sie ein Administrator das Kennwort des Benutzers aktualisieren, ohne die Option zu aktivieren **. Der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern** und das neue Kennwort für den Benutzer freigeben.

3. Das lokales Active Directory User-Objekt ist **nicht ordnungsgemäß** für die Objektsynchronisierung oder Kennwortsynchronisierung konfiguriert. Um dieses Problem zu beheben, führen Sie die Schritte aus, die in der [Problembehandlung für die Kennworthashsynchronisierung mit der Azure AD Connect-Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization) beschrieben sind.







