---
title: Standard-Outlook Bezeichnungseinstellung nicht angewendet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 198ba18365bcd5d1517420890d7a52c4ad8bce17
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65591562"
---
# <a name="default-outlook-label-setting-not-applied"></a>Standard-Outlook Bezeichnungseinstellung nicht angewendet

Wenn Ihre Outlook Standardbezeichnungseinstellungen nicht ordnungsgemäß angewendet werden und eine andere Bezeichnung angewendet wird oder keine Bezeichnung angewendet wird, liegt möglicherweise ein bekanntes Problem (MC277818) vor, und Sie sollten eine der beiden folgenden Optionen ausführen, um das Problem zu beheben:

**Option 1:**

1. Wechseln Sie zu Microsoft Purview-Complianceportal > **Lösungen** >  **Information Protection**.
1. Wählen Sie **"Bezeichnungsrichtlinien**" und dann die Bezeichnungsrichtlinie aus, die Sie bearbeiten müssen (**Die OutlookDefaultlabel-Einstellung** ist für die betreffende Bezeichnungsrichtlinie nicht ordnungsgemäß festgelegt. Führen Sie **"Get-labelpolicy** " aus, um diese Einstellung anzuzeigen, und wählen Sie dann " **Richtlinie bearbeiten"** aus.
1. Wählen Sie **"Weiter**" aus, bis die Einstellung **"Diese Standardbezeichnung auf E-Mails anwenden**" angezeigt wird, die verfügbar ist, wenn Sie im Dialogfeld "**Richtlinieneinstellungen**" die **Option "Benutzer zum Anwenden einer Bezeichnung auf E-Mails und Dokumente des Erben**" auswählen.
1. Wählen Sie im Dialogfeld **"Standardbezeichnung auf Dokumente anwenden** " in der Dropdownliste " **Keine** " aus.
1. Wählen Sie **"Weiter** " und **"Absenden** " aus, um Ihre Bezeichnungseinstellungen zu speichern.

**Option 2:**

Verwenden Sie in [Security and Compliance Center Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps&preserve-view=true) das Set-LabelPolicy-Befehlslet, um **outlookDefaultlabel** in **"None** " im {OutlookDefaultLabel="None"} zu ändern.

Führen Sie Folgendes aus: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Weitere Informationen zu Standardbezeichnungen für Outlook finden [Sie unter Festlegen einer anderen Standardbezeichnung für Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).
