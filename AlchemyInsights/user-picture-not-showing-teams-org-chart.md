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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 27195c6eb88d7e155ed97a888ff3d564ec0c1543
ms.sourcegitcommit: 5afc3c4a1270409ed3691c90ba139878d845e7a3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "66004661"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Benutzerbild wird im Microsoft Teams-Organigramm nicht angezeigt

Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto im Organigramm fehlt, ist es möglich, dass die Einstellung **ShowInAddressLists** auf **False** festgelegt ist:

1. Wechseln Sie zu Microsoft 365 Admin Center > [**Aktive Benutzer**](https://admin.microsoft.com/AdminPortal/Home?ref=users), und wählen Sie den Benutzer mit dem fehlenden Foto aus. 
1. Wählen Sie die Registerkarte **E-Mail** aus, und stellen Sie sicher, dass **In der globalen Adressliste anzeigen** auf **Ja** festgelegt ist.

Wenn das Festlegen von **ShowInAddressLists** auf **Ja** nicht funktioniert, überprüfen Sie Folgendes:

- Der Benutzer ist möglicherweise in der Empfängerliste in Exchange ausgeblendet. Weitere Informationen finden Sie unter [Adressliste in Exchange Online verwalten](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists).
- Der Benutzer ist möglicherweise aus der Adressliste in Azure Active Directory ausgeblendet. Weitere Informationen finden Sie unter [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0&preserve-view=true).
