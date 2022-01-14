---
title: Problembehandlung bei der Registrierung von iOS-Geräten in Microsoft Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 1fa24c601f9781baae111c3bad08559a509d53d3
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61987069"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problembehandlung bei der Registrierung von iOS-Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben. 
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
- **Gerätedeckel erreicht** Der Benutzer verfügt über mehr registrierte Geräte als das Gerätelimit. Überprüfen Sie diese Dokumente, um [ein Gerät](https://docs.microsoft.com/intune/devices-wipe) zu entfernen oder das Gerätelimit zu [ändern.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Dieser Dienst wird nicht unterstützt. Keine Registrierungsrichtlinie:** Der Apple Push Notification Service (APNS) muss konfiguriert oder erneuert werden. Anweisungen dazu finden Sie in [diesem Dokument.](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) 
    
- **Benutzerlizenztyp ungültig oder Benutzername nicht erkannt:** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente, um eine Lizenz über: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) oder [Azure-Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups)zuzuweisen.
    
Zusätzliche Ressourcen zur Behebung Des Problems:
  
1. Verwenden Sie das [Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere Informationen finden Sie in [diesem Dokument.](https://docs.microsoft.com/intune/help-desk-operators) 
    
2. Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Erfahren Sie, wie Sie iOS-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/ios-enroll)
    

