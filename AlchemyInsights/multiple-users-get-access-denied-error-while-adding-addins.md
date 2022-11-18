---
title: Mehrere Benutzer erhalten beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "6700008"
- "5892"
ms.date: 07/23/2020
ms.openlocfilehash: 0d8c0c9313b485adfb4137d226193fd25b6fa9be
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66256834"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Mehrere Benutzer erhalten beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“

Sie können angeben, welche Administratoren in Ihrer Organisation Berechtigungen zum Installieren und Verwalten von Add-Ins für Outlook haben. Außerdem können Sie angeben, welche Benutzer in Ihrer Organisation die Berechtigung zum Installieren und Verwalten von Add-Ins zur eigenen Verwendung besitzen.

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Um zu überprüfen, ob Sie Berechtigungen für einen Benutzer erfolgreich zugewiesen haben, ersetzen Sie \<Role Name\> durch den Namen der Rolle, um dies zu verifizieren, und führen Sie den folgenden Befehl in Exchange Online PowerShell aus:

`Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers`

Dieses Beispiel veranschaulicht, wie Sie verifizieren können, wem Sie Berechtigungen zum Installieren von Add-Ins aus dem Office Store für die Organisation zugewiesen haben.

``` PowerShell
-Role "Org Marketplace Apps" -GetEffectiveUsers
```

Überprüfen Sie in den Ergebnissen `Get-ManagementRoleAssignment` die Einträge in der Spalte „Effektive Benutzer“.

Ausführliche Informationen zu Syntax und Parametern finden Sie unter [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 