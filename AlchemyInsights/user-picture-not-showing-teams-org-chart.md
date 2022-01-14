---
title: Benutzerbild wird im Microsoft Teams-Organigramm nicht angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: b02c8783df614268448a03360cfc7f601af7ee22
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61986600"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Benutzerbild wird im Microsoft Teams-Organigramm nicht angezeigt

Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto im Organigramm fehlt, ist es möglich, dass die Einstellung **ShowInAddressLists** auf **False** festgelegt ist:

1. Wechseln Sie zu Microsoft 365 Admin Center > [**Aktive Benutzer**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), und wählen Sie den Benutzer mit dem fehlenden Foto aus. 
1. Wählen Sie die Registerkarte **E-Mail** aus, und stellen Sie sicher, dass **In der globalen Adressliste anzeigen** auf **Ja** festgelegt ist.

Wenn das Festlegen von **ShowInAddressLists** auf **Ja** nicht funktioniert, überprüfen Sie Folgendes:

- Der Benutzer ist möglicherweise in der Empfängerliste in Exchange ausgeblendet. Weitere Informationen finden Sie unter [Adressliste in Exchange Online verwalten](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists).
- Möglicherweise ist der Benutzer in der Adressliste im Azure Active Directory ausgeblendet. Weitere Informationen finden Sie unter [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0&preserve-view=true).
