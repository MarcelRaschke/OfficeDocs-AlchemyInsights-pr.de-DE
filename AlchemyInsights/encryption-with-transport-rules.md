---
title: Verschlüsselung mit Transportregeln
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079449"
---
# <a name="encryption-with-transport-rules"></a>Verschlüsselung mit Transportregeln

Im [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) können Sie die Funktionen der Office-Nachrichtenverschlüsselung (OME) in ihren Nachrichtenflussregeln verwenden, um die Nachrichtenverschlüsselung auszulösen. Wählen Sie die Option **Office 365-Nachrichtenverschlüsselung und Rechteschutz** in der Transportregelbedingung aus.

- Weitere Informationen finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mails](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Verwenden Sie in PowerShell das Cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities), und legen Sie den Parameter *ApplyOME* auf "$true" fest.
