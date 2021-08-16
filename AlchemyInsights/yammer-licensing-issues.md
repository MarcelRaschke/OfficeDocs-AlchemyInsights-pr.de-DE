---
title: Probleme mit Yammer-Lizenzen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989728"
---
# <a name="yammer-licensing-issues"></a>Probleme mit Yammer-Lizenzen

Jeder Benutzer muss über eine Lizenz verfügen, um den Yammer Enterprise-Dienst zu nutzen, aber Yammer verlangt nicht standardmäßig, dass Benutzer eine Lizenz für den Zugriff auf den Dienst haben. Wenn ein Administrator die Einstellung ändert, um Microsoft 365-Benutzer ohne Yammer-Lizenzen zu blockieren, können Benutzer, denen keine Yammer Enterprise-Lizenz zugewiesen wurde, auf den Yammer-Dienst nicht zugreifen. Weitere Informationen finden Sie unter [Verwalten von Yammer-Benutzerlizenzen in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365). 

Wenn Benutzern Lizenzen entzogen werden, wird die Yammer-Kachel nicht mehr angezeigt, und andere Dienste können die Lizenzentfernung nutzen, um Features auszublenden. In anderen Fällen werden die Features zwar weiterhin angezeigt, zum Verwenden der Features muss aber eine Lizenz zugewiesen werden.  

**Die Lizenz wird für den Benutzer nicht aktualisiert**  

Gelegentlich wurde einem Benutzer eine Lizenz zugewiesen, aber er kann trotzdem nicht auf Yammer zugreifen. Verzögerungen treten eher auf, wenn eine Massenlizenzzuweisung in Bearbeitung ist. Yammer-Benutzer werden möglicherweise nicht in derselben Reihenfolge aktualisiert wie Lizenzen in Azure AD geändert werden, da das System asynchron ausgeführt wird. Warten Sie bis zu 24 Stunden, bevor Sie einen Supportfall öffnen, um Probleme mit der Synchronisierung von Lizenzen zu melden.  

**Massenzuweisung von Lizenzen**  

Lizenzen können über das Admin Center oder PowerShell-Skripts zugewiesen werden. Weitere Informationen finden Sie unter [Zuweisen von Lizenzen an Benutzer](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) und [Zuweisen von Lizenzen zu Benutzerkonten mit Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Der Microsoft-Support bietet keine Unterstützung beim Erstellen von Skripts, aber Dokumentation zu Yammer-Lizenzzuweisungen steht zur Verfügung. Weitere Informationen finden Sie unter [Verwalten von Yammer-Lizenzen mit Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).