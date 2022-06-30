---
title: Verschlüsselung mit Transportregeln
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 126f02d70285024dd8f69ece3f35c51155b7fff5
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66421798"
---
# <a name="encryption-with-transport-rules"></a>Verschlüsselung mit Transportregeln

Im [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) können Sie die Funktionen der Office-Nachrichtenverschlüsselung (OME) in ihren Nachrichtenflussregeln verwenden, um die Nachrichtenverschlüsselung auszulösen. Wählen Sie die Option **Office 365-Nachrichtenverschlüsselung und Rechteschutz** in der Transportregelbedingung aus.

- Weitere Informationen finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mails](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Verwenden Sie in PowerShell das Cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities), und legen Sie den Parameter *ApplyOME* auf "$true" fest.
