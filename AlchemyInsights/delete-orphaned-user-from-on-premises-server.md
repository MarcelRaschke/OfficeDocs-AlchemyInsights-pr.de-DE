---
title: Verwaiste Benutzer vom lokalen Server löschen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 4d4dff959687d91430df12d965911cc398c2ef6b
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61964364"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Verwaiste Benutzer vom lokalen Server löschen

Führen Sie die folgenden Schritte aus, um einen verwaisten Benutzer zu entfernen:

1. Erzwingen Sie die Verzeichnissynchronisierung, indem Sie die Anweisungen in [Was bedeutet Hybrididentität in Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories) befolgen.

2. Um die Verzeichnissynchronisierung zu verifizieren, siehe [Was bedeutet Hybrididentität in Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Wenn die Synchronisierung ordnungsgemäß funktioniert, das Löschen des Active Directory-Objekts jedoch noch nicht an Azure AD weitergegeben wird, können Sie das verwaiste Objekt mithilfe eines der folgenden Azure Active Directory-Module für Windows PowerShell-Cmdlets manuell entfernen:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Wenn Sie beispielsweise die verwaiste Benutzer-ID manuell entfernen möchten, die john.smith@contoso.com ursprünglich mithilfe der Verzeichnissynchronisierung erstellt wurde, führen Sie das folgende Cmdlet aus:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com