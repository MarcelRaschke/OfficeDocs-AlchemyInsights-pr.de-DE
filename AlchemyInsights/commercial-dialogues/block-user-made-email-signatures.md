---
title: Blockieren von vom Benutzer erstellten E-Mail-Signaturen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200009"
- "7310"
ms.date: 12/18/2020
ms.openlocfilehash: 3cab11af70790f7e3ff5f648e13aeb8944c37b1f
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66342849"
---
# <a name="block-user-made-email-signatures"></a>Blockieren von vom Benutzer erstellten E-Mail-Signaturen

Die folgende Lösung gilt nur für E-Mail-Signaturen, die in Outlook im Web erstellt wurden. Sie können Signaturen in der Outlook-App nur blockieren, wenn Sie über eine lokale Exchange Server verfügen.

1. Wählen Sie im Admin Center **Admin Center** > **Exchange** aus.
2. Klicken Sie auf **Berechtigungen** >  **Outlook Web App Richtlinien**.
3. Wählen Sie die Richtlinie aus, und klicken Sie dann auf das Bleistiftsymbol, um sie zu bearbeiten.
4. Klicken Sie auf **"Weitere** > **Optionen"**.
5. Deaktivieren Sie unter **"Benutzererfahrung**" das Kontrollkästchen " **E-Mail-Signatur** ", und klicken Sie dann auf **"Speichern"**.

**Wichtig:** Wenn vor dem Deaktivieren dieses Kontrollkästchens eine Signatur hinzugefügt wurde, kann der Benutzer sie weiterhin verwenden. Bitten Sie ihn, ihn zu entfernen.
