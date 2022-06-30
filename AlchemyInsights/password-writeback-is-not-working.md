---
title: Kennwortrückschreiben funktioniert nicht
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: fbde858a2d4bc2d083b36eeee56d1dfbfb31563f
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66374727"
---
# <a name="password-writeback-is-not-working"></a>Kennwortrückschreiben funktioniert nicht

**Ich habe Probleme beim Konfigurieren des Kennwortrückschreibens**

- Das Kennwortrückschreiben ist ein Premium-Feature.
- Stellen Sie sicher, dass Sie mit den Lizenzierungsanforderungen vertraut sind:
  - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
  - **Nur Cloudbenutzer** – alle Office 365 (O365) kostenpflichtige SKU oder Azure AD Basic
  - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu Lizenzierungsanforderungen finden Sie unter [Lizenzierungsanforderungen für die Self-Service-Kennwortzurücksetzung in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Sie verfügen über mindestens ein Administratorkonto und ein Testbenutzerkonto mit einer der entsprechenden Lizenzen.
- Sie müssen Azure AD Connect mit dem Emulator für den primären Domänencontroller verbinden, damit das Kennwortrückschreiben funktioniert. Sie können Azure AD Connect für die Verwendung eines primären Domänencontrollers konfigurieren, indem Sie mit der rechten Maustaste auf die **Eigenschaften** des Active Directory-Synchronisierungsconnectors klicken und dann **verzeichnispartitionen konfigurieren auswählen**. Suchen Sie von dort aus nach dem Abschnitt **mit den Verbindungseinstellungen des Domänencontrollers** , und aktivieren Sie das Kontrollkästchen mit dem Titel **"Nur bevorzugte Domänencontroller verwenden**".
    **Hinweis**:Wenn es sich bei dem bevorzugten DC nicht um einen PDC-Emulator handelt, greift Azure AD Connect weiterhin auf die PDC zu, um kennwortzurückschreiben.
- Die Kennwortzurücksetzung wurde in Ihrem Mandanten konfiguriert und aktiviert. Weitere Informationen finden Sie unter [Aktivieren von Benutzern zum Zurücksetzen ihrer Azure AD-Kennwörter](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Stellen Sie sicher, dass es sich bei dem Administratorkonto, das zum Aktivieren des Kennwortrückschreibens verwendet wird, um ein Cloudadministratorkonto handelt (das in Azure AD und nicht in lokalem AD erstellt wurde).
- Sie verfügen über eine lokale AD-Bereitstellung mit einer einzelnen oder mehreren Gesamtstrukturen unter Windows Server 2008 R2, Windows Server 2012 oder Windows Server 2012 R2 mit den neuesten installierten Service Packs.
- Sie haben das Azure AD Connect-Tool installiert und Ihre AD-Umgebung für die Synchronisierung mit der Cloud vorbereitet. Stellen Sie vor dem Testen des Kennwortrückschreibens sicher, dass Sie zuerst einen vollständigen Import und eine vollständige Synchronisierung von AD und Azure AD in Azure AD Connect durchführen.
- Wenn Sie mehr erfahren möchten, erfahren Sie, wie Sie eine [vollständige Synchronisierung und einen vollständigen Import in Azure AD Connect durchführen.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Ich habe ein Problem mit der Kennwortrückschreidkonnektivität**

1. Herunterladen und Aktivieren der neuesten Version von [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallkonfiguration: Das Azure AD Connect-Tool (1.1.443 und höher) benötigt **ausgehenden HTTPS-Zugriff** auf:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Zulassen, dass Leerlaufverbindungen mindestens 2-3 Minuten bestehen bleiben

**Ich habe immer noch Probleme mit dem Kennwortrückschreiben**

- Wenn Sie weiterhin Schwierigkeiten haben, versuchen Sie, den Kennwortrückschreibedienst im Azure AD Connect-Tool zu deaktivieren und erneut zu aktivieren.
- Weitere Informationen finden Sie unter [Deaktivieren und erneutes Aktivieren des Kennwortrückschreibens](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
