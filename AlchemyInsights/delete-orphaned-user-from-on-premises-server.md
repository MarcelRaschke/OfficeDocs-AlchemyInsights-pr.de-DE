---
title: Verwaiste Benutzer vom lokalen Server löschen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000179"
- "1725"
ms.date: 07/20/2020
ms.openlocfilehash: 2dfd331d794bc8ef4246d3d51b53ec29805ba746
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66435604"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Verwaiste Benutzer vom lokalen Server löschen

Führen Sie die folgenden Schritte aus, um einen verwaisten Benutzer zu entfernen:

1. Erzwingen Sie die Verzeichnissynchronisierung, indem Sie die Anweisungen in [Was bedeutet Hybrididentität in Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories) befolgen.

2. Um die Verzeichnissynchronisierung zu verifizieren, siehe [Was bedeutet Hybrididentität in Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Wenn die Synchronisierung ordnungsgemäß funktioniert, das Löschen des Active Directory-Objekts jedoch noch nicht an Azure AD weitergegeben wird, können Sie das verwaiste Objekt mithilfe eines der folgenden Azure Active Directory-Module für Windows PowerShell-Cmdlets manuell entfernen:

   - Remove-MsolContact
   - Remove-MsolGroup
   - Remove-MsolUser

   Wenn Sie beispielsweise die verwaiste Benutzer-ID manuell entfernen möchten, die john.smith@contoso.com ursprünglich mithilfe der Verzeichnissynchronisierung erstellt wurde, führen Sie das folgende Cmdlet aus:

   `Remove-MsolUser UserPrincipalName John.Smith@Contoso.com`
