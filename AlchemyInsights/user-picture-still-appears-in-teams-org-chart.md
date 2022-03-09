---
title: Das Benutzerbild erscheint weiterhin im Microsoft Teams Organigramm
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: 9d302515001fcfe2483bf8d17775e420b8abfdeb
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63165090"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Das Benutzerbild erscheint weiterhin im Microsoft Teams Organigramm

Wenn eine oder mehrere Personen in Ihrer Organisation deaktiviert oder entfernt wurden und ihr Profilfoto weiterhin im Organigramm angezeigt wird, ist es möglich, dass die Einstellung **"ShowInAddressLists"** auf "False" festgelegt ist:

1. Wechseln Sie zu Microsoft 365 Admin Center > [Aktive Benutzer](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) und wählen Sie den Benutzer mit dem Foto aus, das weiter angezeigt wird.
1. Wählen Sie die Registerkarte **E-Mail** aus, und stellen Sie sicher, dass **in der globalen Adressliste anzeigen** auf **Nein** festgelegt ist.

Wenn das Festlegen von **ShowInAddressLists** auf **Nein** nicht funktioniert, überprüfen Sie Folgendes:

- Der Benutzer wird möglicherweise aus der Empfängerliste in Exchange angezeigt. Weitere Informationen finden Sie unter [Adressliste in Exchange Online verwalten](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists).
- Der Benutzer wird möglicherweise aus der Adressliste in Azure Active Directory angezeigt. Weitere Informationen finden Sie unter [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0&preserve-view=true).
