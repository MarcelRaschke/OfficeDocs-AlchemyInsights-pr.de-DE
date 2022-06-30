---
title: Informationen zu Yammer-Administratoren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: adaeecc15f9439be52a3808da54d58a1958befe0
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66505107"
---
# <a name="about-yammer-admins"></a>Informationen zu Yammer-Administratoren

**Netzwerkadministratoren**

Globale Administratoren werden automatisch zur Rolle "Überprüfte Admin" in einem Yammer Netzwerk heraufgestuft. In den folgenden Fällen tritt diese Heraufstufung möglicherweise nicht ordnungsgemäß auf:

- Es sind mehrere Yammer Netzwerke vorhanden, und der Administrator wird bei dem falschen angemeldet. [Netzwerkkonsolidierung](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ist erforderlich, um zu einem Yammer Netzwerk zu gelangen.
- Azure PIM wird verwendet. Der Benutzer wird möglicherweise nicht lange genug zum globalen Administrator heraufgestuft, damit die Heraufstufung erfolgt. Ein zukünftiges Update für Yammer kann dieses Problem beheben, aber es empfiehlt sich, Benutzer manuell zum globalen Administrator zu bewerben.
- Ein Synchronisierungsproblem mit dem Yammer Netzwerk ist vorhanden. In diesem Fall ist eine Supportanfrage für weitere Untersuchungen erforderlich.

Weitere Informationen zu Yammer Administratorrollen finden [Sie unter Verwalten Yammer Administratoren](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Gruppenadministratoren**

Gruppenadministratoren für mit Microsoft 365 verbundene Gruppen werden mit der Gruppenmitgliedschaft aus Azure AD synchronisiert. Bei großen Gruppen kann diese Synchronisierung einen längeren Zeitraum dauern.
