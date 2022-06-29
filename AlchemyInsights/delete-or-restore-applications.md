---
title: Löschen oder Wiederherstellen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: a763b70252b8490f0b3719d3952ba551b601f1cc
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66354711"
---
# <a name="delete-or-restore-applications"></a>Löschen oder Wiederherstellen von Anwendungen

**So löschen Sie eine Anwendung aus Ihrem Azure AD-Mandanten**:

1. Wählen Sie im **Azure AD-Portal** **Enterprise-Anwendungen** aus. Suchen Sie dann die Anwendung, die Sie löschen möchten, und wählen Sie sie aus.
2. Wählen Sie im Abschnitt **"Verwalten** " im linken Bereich " **Eigenschaften"** aus.
3. Wählen Sie **"Löschen"** und dann **"Ja** " aus, um zu bestätigen, dass Sie die App aus Ihrem Azure AD-Mandanten löschen möchten.

Weitere Informationen zum Löschen einer App finden Sie in der [Schnellstartanleitung: Löschen einer Anwendung aus Ihrem Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

In PowerShell entfernt das Cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) Anwendungsproxy Konfigurationen aus einer bestimmten Anwendung in Azure Active Directory und kann die Anwendung vollständig löschen, wenn angegeben.

Sie können **eine gelöschte Anwendung** mithilfe von PowerShell wiederherstellen. Sobald die Anwendung, die Sie wiederherstellen möchten, identifiziert wurde, können Sie sie [mithilfe von Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication) wiederherstellen.
