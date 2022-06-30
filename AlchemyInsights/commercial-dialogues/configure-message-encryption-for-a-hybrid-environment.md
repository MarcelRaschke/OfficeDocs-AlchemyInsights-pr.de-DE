---
title: Konfigurieren der Nachrichtenverschlüsselung für eine Hybridumgebung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000078"
- "7342"
ms.date: 02/24/2021
ms.openlocfilehash: 0de5f4549790b4538fed1ee2106db8ee141c35e9
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66414301"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>Konfigurieren der Nachrichtenverschlüsselung für eine Hybridumgebung

In Exchange-Hybridumgebungen können lokale Benutzer verschlüsselte E-Mails nur dann mithilfe der Office-Nachrichtenverschlüsselung (Office Message Encryption, OME) senden, wenn E-Mails über Exchange Online weitergeleitet werden.

Führen Sie die folgenden Schritte aus, um E-Mails mithilfe von OME zu verschlüsseln:

1. Verwenden Sie den Assistenten für die [Hybridkonfiguration](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) , um Ihre Hybridumgebung einzurichten. Für das Einrichten der Verschlüsselung sind keine besonderen Schritte erforderlich.
2. [Richten Sie Ihre Nachrichtenflussregeln für die Verschlüsselung](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) wie gewohnt ein.