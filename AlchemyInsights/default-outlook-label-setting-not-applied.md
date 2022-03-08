---
title: Standardeinstellung Outlook Bezeichnung nicht angewendet
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
ms.openlocfilehash: 53aa5f325b821987ee607e0fc3d72d0ec35e6406
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63299733"
---
# <a name="default-outlook-label-setting-not-applied"></a>Standardeinstellung Outlook Bezeichnung nicht angewendet

Wenn Ihre Outlook Standardbezeichnungseinstellungen nicht ordnungsgemäß angewendet werden und eine andere Bezeichnung oder keine Bezeichnung angewendet wird, tritt möglicherweise ein bekanntes Problem auf (MC277818) und sie sollten eine der beiden folgenden Optionen ausführen, um das Problem zu beheben:

**Option 1:**

1. Wechseln Sie zu Microsoft 365 Compliance Center > **SolutionsInformation** >  **Protection**.
1. Wählen Sie **Bezeichnungsrichtlinien** aus, und wählen Sie die Bezeichnungsrichtlinie aus, die Sie bearbeiten müssen (**Die OutlookDefaultlabel-Einstellung** ist in der betreffenden Bezeichnungsrichtlinie nicht ordnungsgemäß festgelegt. Führen **Sie "Get-labelpolicy"** aus, um diese Einstellung anzuzeigen, und wählen Sie dann **"Richtlinie bearbeiten"** aus.
1. Wählen Sie **"Weiter**" aus, bis die Einstellung "**Diese Standardbezeichnung auf E-Mails anwenden**" angezeigt wird, die verfügbar ist, wenn Sie im Dialogfeld "**Richtlinieneinstellungen**" festlegen, dass **Benutzer eine Bezeichnung auf E-Mails und Dokumente anwenden** müssen.
1. In the **Apply a default label to documents** dialog box, choose **None** from the dropdown list.
1. Wählen Sie **"Weiter** " und **"Übermitteln** " aus, um Ihre Bezeichnungseinstellungen zu speichern.

**Option 2:**

Verwenden Sie in [Security and Compliance Center Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps&preserve-view=true) das Set-LabelPolicy Commandlet, um **die OutlookDefaultlabel** in **"None** " in "{OutlookDefaultLabel="None"} zu ändern.

Führen Sie Folgendes aus: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Weitere Informationen zu Standardbezeichnungen für Outlook finden Sie unter [Festlegen einer anderen Standardbezeichnung für Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).
