---
title: Vorbereiten für die Verwendung von TLS 1.2 in Microsoft 365
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "1600052"
- "1266"
ms.date: 04/21/2020
ms.openlocfilehash: 022b6ace3a8330217f8346ab49a00bd14959766e
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63283013"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Vorbereiten für die Verwendung von TLS 1.2 in Microsoft 365

Ab dem 31. Oktober 2018 setzt Microsoft 365 den Umstieg auf TLS 1.2 fort. Ab dem 15. Oktober 2020 beginnt O365 mit der dienstweiten Einstellung von TLS 1.0 und 1.1. Diese Änderung wird in den nächsten Wochen und Monaten fortgesetzt, aber die Kunden sollten davon ausgehen, dass ab dem 15. Oktober 2020 keine TLS 1.0- und TLS 1.1-Anrufe mit O365 möglich sind. Wie bereits mitgeteilt (MC126199 im Dez. 2017, MC128929 im Feb. 2018, MC186827 im Juli 2019 und MC218794 im Juli 2020), verlagern wir alle unsere Onlinedienste in Transport Layer Security (TLS) 1.2+, um die erstklassige Verschlüsselung zu gewährleisten und sicherzustellen, dass unser Dienst standardmäßig sicherer ist. Kunden können weiterhin auswählen, ob sie TLS 1.0 bzw. 1.1 auf ihren Servern und Ressourcen installieren, doch sollten sie davon ausgehen, dass nur TLS 1.2 und höher funktionieren, wenn sie mit O365-Ressourcen arbeiten.
  
Weitere Informationen zu diesen Änderungen finden Sie [hier](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365) und [hier](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365).
