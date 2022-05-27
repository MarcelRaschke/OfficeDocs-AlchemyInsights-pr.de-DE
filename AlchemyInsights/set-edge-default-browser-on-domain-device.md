---
title: Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: d26ecb90f447e62f2977703123290c1fb0ee38b4
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65727571"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen

Legen Sie Microsoft Edge als Standardbrowser fest:

1. [Erstellen Sie eine Konfigurationsdatei für Standardverknüpfungen](https://go.microsoft.com/fwlink/?linkid=2132437) und speichern Sie sie lokal oder auf einer Netzwerkfreigabe.

1. Öffnen Sie den Gruppenrichtlinien-Editor und gehen Sie dann zu **Computerkonfiguration** > **Administrative Vorlagen** > **Windows-Komponenten** > **Datei-Explorer**.

1. Wählen Sie **Konfigurationsdatei für Standardverknüpfungen festlegen**.

1. Wählen Sie **Richtlinieneinstellung**, und wählen Sie dann **Aktiviert**.

1. Geben Sie unter **Optionen** den Speicherort der Konfigurationsdatei für die Standardverknüpfungen ein und wählen Sie dann **OK**.
