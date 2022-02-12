---
title: Löschen oder Wiederherstellen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 5ce063579e0978ed8da1befd7f0a5705b201ec61
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62735993"
---
# <a name="delete-or-restore-applications"></a>Löschen oder Wiederherstellen von Anwendungen

**So löschen Sie eine Anwendung aus Ihrem Azure AD Mandanten**:

1. Wählen Sie im **Azure AD Portal** **Enterprise Anwendungen** aus. Suchen Sie dann die Anwendung, die Sie löschen möchten, und wählen Sie sie aus.
2. Wählen Sie im Abschnitt **"Verwalten** " im linken Bereich die Option **"Eigenschaften**" aus.
3. Wählen Sie **"Löschen"** und dann **"Ja**" aus, um zu bestätigen, dass Sie die App aus Ihrem Azure AD Mandanten löschen möchten.

Weitere Informationen zum Löschen einer App finden Sie unter [Schnellstart: Löschen einer Anwendung aus Ihrem Azure Active Directory (Azure AD) Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

In PowerShell entfernt das Cmdlet ["Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication)" Anwendungsproxykonfigurationen aus einer bestimmten Anwendung in Azure Active Directory und kann die Anwendung vollständig löschen, wenn angegeben.

Sie können **eine gelöschte Anwendung** mithilfe von PowerShell wiederherstellen. Nachdem die Wiederherstellungsanwendung identifiziert wurde, können Sie sie mit [restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication) wiederherstellen.
