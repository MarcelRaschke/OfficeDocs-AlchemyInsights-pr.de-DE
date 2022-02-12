---
title: Informationen zu Yammer Administratoren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: 90f3324c1604076738877af7a0f874035240010a
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62613191"
---
# <a name="about-yammer-admins"></a>Informationen zu Yammer Administratoren

**Netzwerkadministratoren**

Globale Administratoren werden automatisch zur Rolle "Bestätigter Administrator" in einem Yammer Netzwerk höhergestuft. In den folgenden Fällen wird diese Höherstufung möglicherweise nicht ordnungsgemäß ausgeführt:

- Es sind mehrere Yammer Netzwerke vorhanden, und der Administrator wird beim falschen Netzwerk angemeldet. [Die Netzwerkkonsolidierung](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ist erforderlich, um zu einem Yammer Netzwerk zu gelangen.
- Azure PIM wird verwendet. Der Benutzer wird möglicherweise nicht lange genug zum globalen Administrator höhergestuft, damit die Aktion durchgeführt wird. Ein zukünftiges Update auf Yammer kann dieses Problem beheben, es empfiehlt sich jedoch, Benutzer manuell zum globalen Administrator zu bewerben.
- Beim Yammer-Netzwerk liegt ein Synchronisierungsproblem vor. In diesem Fall ist eine Supportanfrage für die weitere Untersuchung erforderlich.

Weitere Informationen zu Yammer Administratorrollen finden Sie unter [Verwalten Yammer Administratoren](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Gruppenadministratoren**

Gruppenadministratoren für Microsoft 365 verbundene Gruppen werden mit der Gruppenmitgliedschaft von Azure AD synchronisiert. Bei großen Gruppen kann diese Synchronisierung einen längeren Zeitraum dauern.
