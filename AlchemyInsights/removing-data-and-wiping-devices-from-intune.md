---
title: Entfernen von Daten und Zurücksetzen des Geräts aus Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
  - 1279
  - 6700008
  - 9004638
  - 8392
---

# <a name="removing-data-and-wiping-devices-from-intune"></a>Entfernen von Daten und Zurücksetzen des Geräts aus Intune

Die Aktionen "Gerät zurücksetzen" und "Gerät abkoppeln" können verwendet werden, um von Intune verwaltete Unternehmensdaten zu entfernen oder eine Zurücksetzung auf Werkseinstellungen durchzuführen und das Gerät auf seine Standardeinstellungen zurückzusetzen.

1. Melden Sie sich bei der Microsoft 365-Geräteverwaltung an, und navigieren Sie zu **Geräte** > **Alle Geräte**.
2. Wählen Sie das Gerät aus, das Sie zurücksetzen möchten.
3. Wählen Sie die Art der Remotezurücksetzung aus, die Sie durchführen möchten. Durch das Abkoppeln werden nur organisatorische Informationen gelöscht, während eine vollständige Zurücksetzung das Gerät auf die Werkseinstellungen zurücksetzt.
4. Wählen Sie zum Bestätigen **Ja** aus. Bis zum Löschen wird der Status der Geräteaktion als *Abkoppeln ausstehend* angezeigt.
    Nach Abschluss der Aktion wird das mobile Gerät nicht mehr in der Liste der verwalteten Geräte angezeigt.

**Hinweis**: Unternehmensdaten können nicht von Geräten entfernt werden, die mit Azure AD VERBUNDEN sind. 

Ausführliche Informationen zu den Auswirkungen der Aktionen "Abkoppeln" und "Zurücksetzen", einschließlich der beibehaltenen und gelöschten Aktionen, finden Sie in der folgenden Dokumentation:

- [Entfernen Sie Geräte, indem Sie das Gerät zurücksetzen, abkoppeln oder manuell abmelden](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [So löschen Sie nur Unternehmensdaten aus von Intune verwalteten Apps](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Löschen allen Daten von einem MacOS-Gerät](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).