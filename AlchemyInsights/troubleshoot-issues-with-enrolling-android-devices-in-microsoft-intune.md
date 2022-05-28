---
title: Behandeln von Problemen beim Registrieren Android Geräten in Microsoft Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 3b41d17ca23e593926c6cce8db24331bce740903
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65732936"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Behandeln von Problemen beim Registrieren Android Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Probleme und Lösungsschritte:
  
 **Fehler "Gerät nicht verschlüsselt" in Unternehmensportal:** Neuere Versionen von Android, insbesondere ab Version 7.0, erfordern eine Startkennung, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist. Gängige Lösungen sind die Aktivierung einer Start-PIN oder die vollständige Verschlüsselung des Geräts. Lesen Sie [dieses Dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , um weitere Informationen zu erfahren.
  
 **Geräte können nicht mit dem Intune-Dienst einchecken oder in der Intune-Administratorkonsole als "Ungesund" angezeigt werden:** Einige Samsung 4.4- und 5.5-Geräte werden möglicherweise nicht in den Dienst eingecheckt. Es gibt drei mögliche Lösungen für dieses Problem:
  
1. Öffnen Sie manuell die Intune-Unternehmensportal-App, die automatisch eine Gerätesynchronisierung initiiert.

2. Aktualisieren Sie das Gerät auf Android 6.0 oder höher.

3. Deaktivieren Sie Samsung Smart Manager für die Verwaltung der Intune-Unternehmensportal. [In diesem Dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) finden Sie weitere Details zu diesen Problemen und Lösungen.

 Fehler "**Ungültiger Benutzerlizenztyp**" oder **"Benutzername nicht erkannt":** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente, um eine Lizenz zuzuweisen über: Office Admin Center oder Azure-Portal.
  
Zusätzliche Ressourcen zur Behebung Ihres Problems:
  
1. Verwenden Sie [Intune Problembehandlungsportal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade), um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere Details [finden Sie in diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) .

2. Überprüfen Sie [dieses Dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) auf eine Liste der häufig auftretenden Fehler, die registrierungs- und lösungsbehebungen für jeden verhindern.

3. [Erfahren Sie, wie Sie Android Geräte in Microsoft Intune registrieren](https://docs.microsoft.com/intune/android-enroll).
