---
title: Hilfe für die Anzeigeeinstellungen des Nachtmodus
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: 8d1f979b03b1257dbe5d5f309548aee33134a779
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63275957"
---
# <a name="help-with-the-night-light-display-setting"></a>Hilfe für die Anzeigeeinstellungen des Nachtmodus

Weitere Informationen über die Anzeigeeinstellungen des Nachtmodus finden Sie unter [Einrichten der Anzeige für die Nacht in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Wenn die Optionen für den Nachtmodus in den Einstellungen abgeblendet sind, überprüfen Sie Ihren Bildschirmtreiber: 

1. Klicken Sie in das Suchfeld in Ihrer Taskleiste und geben Sie **Geräte-Manager** ein und wählen Sie dann **Geräte-Manager** in den Suchergebnissen aus.
1. Erweitern Sie **Bildschirm-Adapter**. 

Leider ist die Nachtmodusfunktion nicht verfügbar, wenn Ihr Gerät einen DisplayLink-Treiber oder einen Standard-Bildschirmtreiber verwendet.

Die Nachtmodusfunktion verwendet die neueste Grafiktechnologie, sodass Sie möglicherweise Ihren Bildschirmtreiber aktualisieren müssen:  

- Überprüfen Sie auf Updates, indem Sie zu **Start** > **Einstellungen** > **Update und Sicherheit** > **Windows Update** > **Nach Updates suchen** wechseln.  

ODER

- Besuchen Sie die Support-Website Ihres Hardwareherstellers, um die neuesten Bildschirmtreiber manuell herunterzuladen und zu installieren.

## <a name="reset-night-light-in-the-registry"></a>Setzen Sie den Nachtmodus in der Registrierung zurück.

Wenn die Aktualisierung Ihres Anzeigetreibers nicht funktioniert hat, müssen Sie möglicherweise den Nachtmodus in der Registrierung zurücksetzen.  

**Vorsicht**: Dieser Problembehandlungsschritt wird nur fortgeschrittenen Benutzer empfohlen. Durch eine fehlerhafte Bearbeitung der Registrierung können schwerwiegende Probleme verursacht werden. Sichern Sie für zusätzlichen Schutz die Registrierung, bevor Sie diese ändern, damit sie bei Problemen wiederhergestellt werden kann.

1. Geben Sie im Suchfeld **regedit** ein, und wählen Sie den **Registrierungs-Editor** in den Suchergebnissen aus.

1. Navigieren Sie zu folgendem Registrierungsschlüssel: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exportieren und Löschen Sie danach den folgenden Eintrag subkey:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exportieren und Löschen Sie danach den folgenden Eintrag subkey:$$windows.data.bluelightreduction.settings

1. Starten Sie Windows neu und verifizieren Sie, dass die Optionen für den Nachtmodus verfügbar sind.


