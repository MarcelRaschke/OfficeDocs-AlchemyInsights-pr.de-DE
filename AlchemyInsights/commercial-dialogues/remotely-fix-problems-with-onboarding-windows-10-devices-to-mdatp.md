---
title: Remotebehebung von Problemen beim Onboarding Windows 10 Geräten in Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: f3d633aa784316cc71d623f48a462ca5f7485beb
ms.sourcegitcommit: f3903d6919d46a31a38edef25d9717a6d005bb15
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2022
ms.locfileid: "65395693"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Remotebehebung von Problemen beim Onboarding Windows 10 Geräten in Microsoft Defender Advanced Threat Protection

Wenn Sie auf den Remotecomputer zugreifen können, führen Sie die folgenden Schritte aus:

1. Laden Sie das [Clientverbindungsuntersuchung](https://go.microsoft.com/fwlink/?linkid=2143466)-Diagnosetool herunter.
2. Extrahieren Sie MDATPAnalyzer.cmd, und führen Sie es aus.
3. Suchen Sie das Diagnoseprotokoll im Ordner "MDATPClientAnalyzerResult", demselben Ordner, in den das Analysetool heruntergeladen wurde.
4. Um Probleme mit Denk- oder Internetproxyeinstellungen zu finden, überprüfen Sie die Protokolldatei MDATPClientAnalyzer.txt.

Weitere Informationen finden Sie [unter Probleme mit Onboarding-Computern](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/troubleshoot-onboarding).
