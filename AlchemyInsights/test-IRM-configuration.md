---
title: IRM-Konfiguration für neue HOME-Funktionen testen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: aa9368cb9a621f043d1a67766e502c9983730f29
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62742455"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>IRM-Konfiguration für neue HOME-Funktionen testen

Um zu überprüfen, ob Ihr Microsoft 365-Mandant für die Verwendung neuer OME-Funktionen konfiguriert ist, führen Sie die folgenden Cmdlets aus, während Sie mit [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell) verbunden sind:


1. Überprüfen Sie die IRM-Konfiguration Ihres Mandanten, indem Sie `Get-IRMConfiguration` ausführen. Stellen Sie sicher, dass diese Werte auf **True** gesetzt sind:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Führen Sie mit Ihrer Domain, Absenderadresse und Empfänger `Test-IRMConfiguration` aus. Wenn der Test nicht bestanden wird, untersuchen Sie Ihre IRM-Konfiguration.

Weitere Informationen zum Überprüfen der IRM-Konfiguration finden Sie unter [Überprüfen der neuen OME-Konfiguration in Exchange Online PowerShell](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).