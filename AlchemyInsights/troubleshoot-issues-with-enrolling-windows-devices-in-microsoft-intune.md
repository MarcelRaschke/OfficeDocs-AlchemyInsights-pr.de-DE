---
title: Problembehandlung bei der Registrierung Windows Geräten in Microsoft Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 66de74cab5972ffc4318965ede4f7b84721541ba
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61831670"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problembehandlung bei der Registrierung Windows Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
 **Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen. Laden Sie das PC-Clientsoftwarepaket in der Intune Admin Console erneut herunter. Weitere Informationen hierzu in dieser Dokumentation.
  
 **Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:
  
-  Der Benutzer verfügt über mehr registrierte Geräte als das Gerätelimit. Überprüfen Sie diese Dokumente, um [ein Gerät](https://docs.microsoft.com/intune/devices-wipe) zu entfernen oder das Gerätelimit zu [ändern.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Benutzer können Geräte mit Azure AD verbinden" ist auf "none" festgelegt. Legen Sie es auf alle oder ausgewählte Benutzer fest. Weitere Informationen hierzu in [dieser Dokumentation.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)

-  Das Gerät ist bereits von einem anderen Benutzer registriert. Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure Intune-Konsole, oder heben Sie die Registrierung des Geräts manuell auf, bevor Sie es erneut versuchen.

-  Das Gerät ist Windows 10 Home. Nur Windows 10 Pro, Education und Enterprise SKUs können Azure Active Directory beitreten.

Zusätzliche Ressourcen zur Behebung Des Problems:
  
-  Verwenden Sie das [Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere Informationen finden Sie in [diesem Dokument.](https://docs.microsoft.com/intune/help-desk-operators)

-  Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Erfahren Sie, wie Sie Windows Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/windows-enroll)
