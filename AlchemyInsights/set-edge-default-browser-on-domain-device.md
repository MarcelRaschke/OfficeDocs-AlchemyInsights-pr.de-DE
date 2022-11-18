---
title: Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9006005"
- "10362"
ms.date: 03/29/2021
ms.openlocfilehash: b0efb0fbc14ac00d576aa908511cd59909322014
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66417910"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen

Legen Sie Microsoft Edge als Standardbrowser fest:

1. [Erstellen Sie eine Konfigurationsdatei für Standardverknüpfungen](https://go.microsoft.com/fwlink/?linkid=2132437) und speichern Sie sie lokal oder auf einer Netzwerkfreigabe.

1. Öffnen Sie den Gruppenrichtlinien-Editor und gehen Sie dann zu **Computerkonfiguration** > **Administrative Vorlagen** > **Windows-Komponenten** > **Datei-Explorer**.

1. Wählen Sie **Konfigurationsdatei für Standardverknüpfungen festlegen**.

1. Wählen Sie **Richtlinieneinstellung**, und wählen Sie dann **Aktiviert**.

1. Geben Sie unter **Optionen** den Speicherort der Konfigurationsdatei für die Standardverknüpfungen ein und wählen Sie dann **OK**.
