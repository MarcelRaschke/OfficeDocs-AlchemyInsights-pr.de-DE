---
title: IRM-Konfiguration für neue HOME-Funktionen testen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000078"
- "12428"
ms.date: 07/19/2021
ms.openlocfilehash: 1ebd4ba618138c1d1d5ed819c29fc026c6c2e23f
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66261910"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>IRM-Konfiguration für neue HOME-Funktionen testen

Um zu überprüfen, ob Ihr Microsoft 365-Mandant für die Verwendung neuer OME-Funktionen konfiguriert ist, führen Sie die folgenden Cmdlets aus, während Sie mit [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell) verbunden sind:


1. Überprüfen Sie die IRM-Konfiguration Ihres Mandanten, indem Sie `Get-IRMConfiguration` ausführen. Stellen Sie sicher, dass diese Werte auf **True** gesetzt sind:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Führen Sie mit Ihrer Domain, Absenderadresse und Empfänger `Test-IRMConfiguration` aus. Wenn der Test nicht bestanden wird, untersuchen Sie Ihre IRM-Konfiguration.

Weitere Informationen zum Überprüfen der IRM-Konfiguration finden Sie unter [Überprüfen der neuen OME-Konfiguration in Exchange Online PowerShell](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).