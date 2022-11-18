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
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 641a021f22484e84832df1647e636e78938f95c5
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66356943"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Remotebehebung von Problemen beim Onboarding Windows 10 Geräten in Microsoft Defender Advanced Threat Protection

Wenn Sie auf den Remotecomputer zugreifen können, führen Sie die folgenden Schritte aus:

1. Laden Sie das [Clientverbindungsuntersuchung](https://go.microsoft.com/fwlink/?linkid=2143466)-Diagnosetool herunter.
2. Extrahieren Sie MDATPAnalyzer.cmd, und führen Sie es aus.
3. Suchen Sie das Diagnoseprotokoll im Ordner "MDATPClientAnalyzerResult", demselben Ordner, in den das Analysetool heruntergeladen wurde.
4. Um Probleme mit Denk- oder Internetproxyeinstellungen zu finden, überprüfen Sie die Protokolldatei MDATPClientAnalyzer.txt.

Weitere Informationen finden Sie [unter Probleme mit Onboarding-Computern](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/troubleshoot-onboarding).
