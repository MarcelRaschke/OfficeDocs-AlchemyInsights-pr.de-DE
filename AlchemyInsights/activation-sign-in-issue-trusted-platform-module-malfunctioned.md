---
title: Aktivierungs-/Anmeldeproblem – Vertrauenswürdiges Plattformmodul nicht ordnungsgemäß funktioniert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 4e302dc0d00b681112128e1a7b71c9a6255095ab
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62563311"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Beheben der Meldung "Das Trusted Platform-Modul Ihres Computers funktioniert nicht ordnungsgemäß" Microsoft 365 Apps

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

1. Öffnen Sie eine Office-App, und [melden Sie sich von vorhandenen Benutzerkonten ab](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071).   
2. Entfernen Sie vorhandene Geschäftskonten **mithilfe Windows Einstellungen** >  **AccountsEmail** > **-& Konten**. 
3. Trennen Sie vorhandene Konten mithilfe **Windows Einstellungen** >  **KontosAccess-Geschäfts** > -, **Schul- oder Unikontos**. 
4. Setzen Sie den Office-Aktivierungsstatus zurück. [Anleitung](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Versuchen Sie den [Benutzerwiederherstellungsprozess](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , um TPM-Fehler (Trusted Platform Module) zu beheben.