---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031261"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Veraltete ausgehende EOP-IP-Adressbereiche

Wir haben ein potenzielles Problem mit Ihrer Organisation erkannt, das (wenn es nicht bis zum 26. Oktober 2018 behoben wurde) möglicherweise den Nachrichtenfluss zu Ihren lokalen oder externen Zielen unterbricht. Wie bereits erwähnt, konsolidieren wir zur Vereinfachung der Verwaltung des IP-Adressbereichs die ip-Adressbereiche Exchange Online Protection (EOP), die zum Senden und Empfangen von E-Mails außerhalb von Microsoft 365 verwendet werden. Unsere Analyse weist darauf hin, dass eine oder mehrere der externen E-Mail-Quellen oder Ziele, die Sie in E-Mail-Flussconnectors konfiguriert haben, keine Verbindungen aus den [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)gezeigten IP-Adressbereichen akzeptieren.

Handeln Sie vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zu und von allen [veröffentlichten EOP-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)akzeptieren.

Weitere Informationen zu dieser Änderung finden Sie in den Nachrichtencenterbeiträgen [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Hinweis:** Wenn Sie zuvor die IP- oder URL-Veröffentlichung über HTML, XML und RSS für Endpunktupdates verwendet haben, sollten Sie auch zu den neuen Webdiensten migrieren, um diese Arten von Updates zu automatisieren. Weitere Informationen finden Sie unter [Microsoft 365 Endpunktkategorien und Microsoft 365 IP-Adresse und URL-Webdienst.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
