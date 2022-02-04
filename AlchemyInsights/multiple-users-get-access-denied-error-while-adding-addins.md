---
title: Mehrere Benutzer erhalten beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
  - 5892
  - 6700008
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
 