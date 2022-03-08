---
title: Löschen oder Wiederherstellen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 65e93813ff8c59fae019ec12cda0786f93c9a260
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63130169"
---
# <a name="delete-or-restore-applications"></a>Löschen oder Wiederherstellen von Anwendungen

**So löschen Sie eine Anwendung aus Ihrem Azure AD Mandanten**:

1. Wählen Sie im **Azure AD Portal** **Enterprise Anwendungen** aus. Suchen Sie dann die Anwendung, die Sie löschen möchten, und wählen Sie sie aus.
2. Wählen Sie im Abschnitt **"Verwalten** " im linken Bereich die Option **"Eigenschaften**" aus.
3. Wählen Sie **"Löschen"** und dann **"Ja**" aus, um zu bestätigen, dass Sie die App aus Ihrem Azure AD Mandanten löschen möchten.

Weitere Informationen zum Löschen einer App finden Sie unter [Schnellstart: Löschen einer Anwendung aus Ihrem Azure Active Directory (Azure AD) Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

In PowerShell entfernt das Cmdlet ["Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication)" Anwendungsproxykonfigurationen aus einer bestimmten Anwendung in Azure Active Directory und kann die Anwendung vollständig löschen, wenn angegeben.

Sie können **eine gelöschte Anwendung** mithilfe von PowerShell wiederherstellen. Nachdem die Wiederherstellungsanwendung identifiziert wurde, können Sie sie mit [restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication) wiederherstellen.
