---
title: Problembehandlung bei der Kennwortsynchronisierung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1300006"
- "579"
ms.date: 04/21/2020
ms.openlocfilehash: e2801b9bbe6db0464a1f26395cb44a491db4656d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66360615"
---
# <a name="troubleshoot-password-synchronization"></a>Problembehandlung bei der Kennwortsynchronisierung

Um Probleme mit der Kennwortsynchronisierung zu beheben, verwenden Sie zunächst diese AAD Connect-Problembehandlungsaufgabe, um zu ermitteln, warum Kennwörter nicht synchronisiert werden. Wechseln Sie zunächst zu ["Direkte Synchronisierung verwalten](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)".  

1. Öffnen Sie eine neue Windows PowerShell-Sitzung auf Ihrem Azure AD Connect-Server, und wählen Sie die Option **"Als Administrator ausführen" aus**.

2. Führen Sie Set-ExecutionPolicy RemoteSigned oder Set-ExecutionPolicy Unrestricted aus.

3. Starten Sie den Azure AD Connect-Assistenten.

4. Wechseln Sie zur Seite "Weitere Aufgaben", > **"Nächste Problembehandlung"** > .

5. Wählen Sie **"Starten** " aus, um das PowerShell-Menü zur Problembehandlung zu öffnen.

6. Wählen Sie **Problembehandlung bei der Kennwortsynchronisierung aus**.

    Das Problem besteht in der Regel darin, dass ein Kennwort für ein bestimmtes Benutzerkonto nicht synchronisiert wird.

    **Notizen** Die Kennwortsynchronisierung schlägt fehl, wenn die letzte erfolgreiche Kennwortsynchronisierung vor einiger Zeit erfolgte.

Weitere Hilfe zur Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennworthashsynchronisierung mit der Azure AD Connect-Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).