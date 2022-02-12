---
title: Kennwortrückschreiben funktioniert nicht
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: c9d96da7d7f9bf257ff798c0b25e313948db60c3
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62634126"
---
# <a name="password-writeback-is-not-working"></a>Kennwortrückschreiben funktioniert nicht

**Ich habe Probleme beim Konfigurieren des Kennwortrückschreibens**

- Das Kennwortrückschreiben ist ein Premium-Feature.
- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:
  - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
  - **Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365) oder Azure AD Basic
  - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu den Lizenzierungsanforderungen finden Sie unter ["Lizenzierungsanforderungen für Azure AD Self-Service-Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)".
- Sie verfügen über mindestens ein Administratorkonto und ein Testbenutzerkonto mit einer der entsprechenden Lizenzen.
- Sie müssen Azure AD Verbinden mit dem primären Domänencontroller Emulator verbinden, damit das Kennwortrückschreiben funktioniert. Sie können Azure AD Verbinden für die Verwendung eines primären Domänencontrollers konfigurieren, indem Sie mit der rechten Maustaste auf die **Eigenschaften** des Active Directory-Synchronisierungsconnectors klicken und dann **Verzeichnispartitionen konfigurieren** auswählen. Suchen Sie dort nach dem Abschnitt " **Domänencontroller-Verbindungseinstellungen** ", und aktivieren Sie das Kontrollkästchen, in dem **nur bevorzugte Domänencontroller verwendet werden**.
    **Hinweis**:Wenn es sich bei dem bevorzugten DC nicht um einen PDC-Emulator handelt, Azure AD Verbinden weiterhin den PDC für das Kennwortrückschreiben erreichen.
- Die Kennwortzurücksetzung wurde in Ihrem Mandanten konfiguriert und aktiviert. Weitere Informationen finden Sie unter [Aktivieren von Benutzern, ihre Azure AD Kennwörter zurückzusetzen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Stellen Sie sicher, dass es sich bei dem Administratorkonto, das zum Aktivieren des Kennwortrückschreibens verwendet wird, um ein Cloudadministratorkonto handelt (das in Azure AD nicht im lokalen AD erstellt wurde).
- Sie verfügen über eine lokale AD-Bereitstellung mit einer oder mehreren Gesamtstrukturen, die Windows Server 2008 R2, Windows Server 2012 oder Windows Server 2012 R2 mit den neuesten installierten Service Packs ausgeführt wird.
- Sie haben das Azure AD Verbinden-Tool installiert und Ihre AD-Umgebung für die Synchronisierung in der Cloud vorbereitet. Stellen Sie vor dem Testen des Kennwortrückschreibens sicher, dass Sie zuerst einen vollständigen Import und eine vollständige Synchronisierung aus AD und Azure AD in Azure AD Verbinden durchführen.
- Weitere Informationen finden Sie unter "[Vollständige Synchronisierung und vollständiger Import" in Azure AD Verbinden](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Ich habe ein Problem mit der Kennwortrückschreibkonnektivität**

1. Herunterladen und Aktivieren der neuesten Version von [Azure AD Verbinden](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallkonfiguration: Das Azure AD Verbinden-Tool (1.1.443 und höher) benötigt **ausgehenden HTTPS-Zugriff** auf:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Zulassen, dass Leerlaufverbindungen mindestens 2-3 Minuten lang bestehen bleiben

**Ich habe weiterhin Probleme mit dem Kennwortrückschreiben**

- Wenn Sie weiterhin Probleme haben, versuchen Sie, den Kennwortrückschreibdienst im tool Azure AD Verbinden zu deaktivieren und erneut zu aktivieren.
- Weitere Informationen finden Sie unter ["Deaktivieren und erneutes Aktivieren des Kennwortrückschreibens](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)"
