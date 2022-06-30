---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 1065
ms.date: 04/21/2020
ms.openlocfilehash: 89f7e10e9069f6cacf27802f1675736cf02ddddf
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66527052"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation of EOP outbound IP address ranges

Wir haben ein potenzielles Problem mit Ihrer Organisation erkannt, das (wenn nicht bis zum 26. Oktober 2018 korrigiert) den Nachrichtenfluss an Ihre lokalen oder externen Ziele unterbrechen könnte. Wie bereits kommuniziert, konsolidieren wir zur Vereinfachung der VERWALTUNG von IP-Adressbereichen die EXCHANGE ONLINE PROTECTION (EOP)-IP-Adressbereiche, die zum Senden und Empfangen von E-Mails außerhalb von Microsoft 365 verwendet werden. Unsere Analyse weist darauf hin, dass eine oder mehrere externe E-Mail-Quellen oder Ziele, die Sie in Nachrichtenflussconnectors konfiguriert haben, keine Verbindungen aus bestimmten IP-Adressbereichen akzeptieren.

Handeln Sie vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zu und von allen [veröffentlichten EOP-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses) akzeptieren.

Weitere Informationen zu dieser Änderung finden Sie in den Nachrichtencenter-Beiträgen [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620) oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Hinweis**: Wenn Sie zuvor die IP- oder URL-Veröffentlichung über HTML, XML und RSS für Endpunktupdates verwendet haben, sollten Sie auch zu den neuen Webdiensten migrieren, um diese Arten von Updates zu automatisieren. Weitere Informationen finden Sie unter [Microsoft 365-Endpunktkategorien und Microsoft 365-IP-Adresse und URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
