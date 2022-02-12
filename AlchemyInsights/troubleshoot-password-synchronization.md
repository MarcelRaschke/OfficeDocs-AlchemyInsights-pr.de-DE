---
title: Problembehandlung bei der Kennwortsynchronisierung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 207d4f512efd96a776004ca28988568db9e16364
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62583165"
---
# <a name="troubleshoot-password-synchronization"></a>Problembehandlung bei der Kennwortsynchronisierung

Um Probleme mit der Kennwortsynchronisierung zu beheben, verwenden Sie zunächst diese AAD Verbinden Problembehandlungsaufgabe, um zu ermitteln, warum Kennwörter nicht synchronisiert werden. Wechseln Sie zunächst zu ["Direkte Synchronisierung verwalten"](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Öffnen Sie eine neue Windows PowerShell Sitzung auf Ihrem Azure AD Verbinden Server, und wählen Sie die Option **"Als Administrator ausführen**" aus.

2. Führen Sie Set-ExecutionPolicy RemoteSigned oder Set-ExecutionPolicy Uneingeschränkt aus.

3. Starten Sie den Assistenten Azure AD Verbinden.

4. Wechseln Sie zur Seite "Zusätzliche Aufgaben" > **Problembehandlung** > **.**

5. Wählen Sie **"Start** " aus, um das PowerShell-Menü zur Problembehandlung zu öffnen.

6. Wählen Sie **Problembehandlung bei der Kennwortsynchronisierung aus**.

    Das Problem besteht in der Regel darin, dass ein Kennwort für ein bestimmtes Benutzerkonto nicht synchronisiert wird.

    **Notizen** Bei der Kennwortsynchronisierung tritt ein Fehler auf, wenn die letzte erfolgreiche Kennwortsynchronisierung einige Zeit zurückliegt.

Weitere Hilfe zur Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennworthashsynchronisierung mit Azure AD Verbinden Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).