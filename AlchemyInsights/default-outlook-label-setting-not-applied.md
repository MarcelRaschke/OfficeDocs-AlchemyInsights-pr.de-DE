---
title: Outlook-Standardbezeichnungseinstellung nicht angewendet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000181"
- "13259"
ms.date: 8/16/2021
ms.openlocfilehash: a1aa81d1332458a6d6aeb4f192b40a84a5ef7c43
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66422554"
---
# <a name="default-outlook-label-setting-not-applied"></a>Outlook-Standardbezeichnungseinstellung nicht angewendet

Wenn Ihre Outlook-Standardbezeichnungseinstellungen nicht ordnungsgemäß angewendet werden und eine andere Bezeichnung oder keine Bezeichnung angewendet wird, liegt möglicherweise ein bekanntes Problem (MC277818) vor, und Sie sollten eine der beiden folgenden Optionen ausführen, um das Problem zu beheben:

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
