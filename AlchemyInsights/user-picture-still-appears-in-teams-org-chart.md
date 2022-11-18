---
title: Das Benutzerbild erscheint weiterhin im Microsoft Teams Organigramm
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9007457"
- "13834"
ms.date: 09/13/2021
ms.openlocfilehash: f6063f53637ff35319e1abf2b308aa6232fcbe6c
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66512724"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Das Benutzerbild erscheint weiterhin im Microsoft Teams Organigramm

Wenn eine oder mehrere Personen in Ihrer Organisation deaktiviert oder entfernt wurden und ihr Profilfoto weiterhin im Organigramm angezeigt wird, ist es möglich, dass die Einstellung **"ShowInAddressLists"** auf "False" festgelegt ist:

1. Wechseln Sie zu Microsoft 365 Admin Center > [Aktive Benutzer](https://admin.microsoft.com/AdminPortal/Home?ref=users) und wählen Sie den Benutzer mit dem Foto aus, das weiter angezeigt wird.
1. Wählen Sie die Registerkarte **E-Mail** aus, und stellen Sie sicher, dass **in der globalen Adressliste anzeigen** auf **Nein** festgelegt ist.

Wenn das Festlegen von **ShowInAddressLists** auf **Nein** nicht funktioniert, überprüfen Sie Folgendes:

- Der Benutzer wird möglicherweise aus der Empfängerliste in Exchange angezeigt. Weitere Informationen finden Sie unter [Adressliste in Exchange Online verwalten](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists).
- Der Benutzer wird möglicherweise aus der Adressliste in Azure Active Directory angezeigt. Weitere Informationen finden Sie unter [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0&preserve-view=true).
