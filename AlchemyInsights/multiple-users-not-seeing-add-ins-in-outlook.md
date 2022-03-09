---
title: Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 04914cc3a4e5f577efad6abc0d617b59bd74e5dd
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63264005"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt

Wenn Sie Outlook-Add-Ins testen und keine angezeigt werden, verwenden Sie als ersten Schritt zur Problembehandlung das PowerShell-Cmdlet **Get-OrganizationConfig**, um den Parameter _AppsForOffice Enabled_ abzufragen. Wenn die Abfrage den Wert **False** zurückgibt, setzen Sie diesen Parameter mit dem Cmdlet **Set-OrganizationConfig** auf **True**, damit Add-Ins wie erwartet angezeigt werden.

Es wird nicht empfohlen, den Parameter _AppsForOfficeEnabled_ auf **False** festzulegen. Der Wert **False** überschreibt alle oben genannten Administrator- und Benutzerrolleneinstellungen und verhindert, dass neue Apps von Benutzern in der Organisation aktiviert werden.

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).