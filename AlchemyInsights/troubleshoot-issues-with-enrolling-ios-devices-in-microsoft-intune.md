---
title: Behandeln von Problemen bei der Registrierung von iOS-Geräten in Microsoft Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 3b869708486c25e1a2af37dc1beb8c9c1c1ed8a1
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66396255"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Behandeln von Problemen bei der Registrierung von iOS-Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben. 
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
- **Gerätekappe erreicht** Der Benutzer hat mehr Geräte registriert als der Gerätegrenzwert. Überprüfen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [das Gerätelimit zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Der Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden. In [diesem Dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) finden Sie Anweisungen dazu. 
    
- **Ungültiger Benutzerlizenztyp oder Nicht erkannter Benutzername:** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente, um eine Lizenz zuzuweisen über: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder [Azure-Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Zusätzliche Ressourcen zur Behebung Ihres Problems:
  
1. Verwenden Sie [Intune Problembehandlungsportal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade), um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere Details [finden Sie in diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Erfahren Sie, wie Sie iOS-Geräte in Microsoft Intune registrieren](https://docs.microsoft.com/intune/ios-enroll).
    

