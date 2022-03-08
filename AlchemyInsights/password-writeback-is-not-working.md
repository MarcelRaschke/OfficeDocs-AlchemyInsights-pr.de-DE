---
title: Kennwortrückschreiben funktioniert nicht
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: 471bcf1b075127939d396e9bb840965d5ec2f3ce
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63158395"
---
# <a name="password-writeback-is-not-working"></a>Kennwortrückschreiben funktioniert nicht

**Ich habe Probleme beim Konfigurieren des Kennwortrückschreibens**

- Das Kennwortrückschreiben ist ein Premium-Feature.
- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:
  - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
  - **Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365)-SKU oder Azure AD Basic
  - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu den Lizenzierungsanforderungen finden Sie unter ["Lizenzierungsanforderungen für die Azure AD Self-Service-Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)".
- Sie verfügen über mindestens ein Administratorkonto und ein Testbenutzerkonto mit einer der entsprechenden Lizenzen.
- Sie müssen Azure AD Connect mit dem Emulator für den primären Domänencontroller verbinden, damit das Kennwortrückschreiben funktioniert. Sie können Azure AD Connect für die Verwendung eines primären Domänencontrollers konfigurieren, indem Sie mit der rechten Maustaste auf die **Eigenschaften** des Active Directory-Synchronisierungsconnectors klicken und dann **Verzeichnispartitionen konfigurieren** auswählen. Suchen Sie dort nach dem Abschnitt " **Domänencontroller-Verbindungseinstellungen** ", und aktivieren Sie das Kontrollkästchen, in dem **nur bevorzugte Domänencontroller verwendet werden**.
    **Hinweis**: Wenn es sich bei dem bevorzugten DC nicht um einen PDC-Emulator handelt, erreicht Azure AD Connect weiterhin den PDC, um das Kennwortrückschreiben zu erhalten.
- Die Kennwortzurücksetzung wurde in Ihrem Mandanten konfiguriert und aktiviert. Weitere Informationen finden Sie unter [Aktivieren von Benutzern zum Zurücksetzen ihrer Azure AD-Kennwörter](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Stellen Sie sicher, dass es sich bei dem Administratorkonto, das zum Aktivieren des Kennwortrückschreibens verwendet wird, um ein Cloudadministratorkonto handelt (das in Azure AD nicht im lokalen AD erstellt wurde).
- Sie verfügen über eine lokale AD-Bereitstellung mit einer oder mehreren Gesamtstrukturen unter Windows Server 2008 R2, Windows Server 2012 oder Windows Server 2012 R2, in der die neuesten Service Packs installiert sind.
- Sie haben das Azure AD Connect-Tool installiert und Ihre AD-Umgebung für die Synchronisierung in der Cloud vorbereitet. Stellen Sie vor dem Testen des Kennwortrückschreibens sicher, dass Sie zuerst einen vollständigen Import und eine vollständige Synchronisierung von AD und Azure AD in Azure AD Connect durchführen.
- Weitere Informationen finden Sie unter " [Vollständige Synchronisierung und vollständiger Import" in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Ich habe ein Problem mit der Kennwortrückschreibkonnektivität**

1. Herunterladen und Aktivieren der neuesten Version von [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallkonfiguration: Das Azure AD Connect-Tool (1.1.443 und höher) benötigt **ausgehenden HTTPS-Zugriff** auf:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Zulassen, dass Leerlaufverbindungen mindestens 2-3 Minuten lang bestehen bleiben

**Ich habe weiterhin Probleme mit dem Kennwortrückschreiben**

- Wenn Sie weiterhin Probleme haben, versuchen Sie, den Kennwortrückschreibdienst im Azure AD Connect-Tool zu deaktivieren und erneut zu aktivieren.
- Weitere Informationen finden Sie unter ["Deaktivieren und erneutes Aktivieren des Kennwortrückschreibens](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)"
