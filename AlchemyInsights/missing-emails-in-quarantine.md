---
title: Fehlende E-Mails in Quarantäne
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
  - 5668
  - 9002625
---
# <a name="missing-emails-in-quarantine"></a>Fehlende E-Mails in Quarantäne

Administratoren können [diese Nachrichten anzeigen, freigeben oder löschen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Wechseln Sie im portal Microsoft 365 Defender unter <https://security.microsoft.com> **"Quarantäne überprüfen".** \>  Oder verwenden Sie , um direkt zur **Quarantäneseite** zu <https://security.microsoft.com/quarantine> wechseln.  

Weitere Informationen zu den Such-/Filterwerten, die Sie verwenden können, finden Sie unter [Verwalten von isolierten Nachrichten und Dateien als Administrator in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Die Cmdlets, die Sie zum Anzeigen und Verwalten von Nachrichten und Dateien in Quarantäne verwenden, sind:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Beachten Sie, dass dieses Cmdlet nur für Nachrichten gilt, nicht für Dateien aus Tresor Anlagen für SharePoint, OneDrive oder Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
