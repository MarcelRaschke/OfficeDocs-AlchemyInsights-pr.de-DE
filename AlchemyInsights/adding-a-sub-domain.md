---
title: Hinzufügen einer Unterdomäne
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "13902"
- "7"
ms.openlocfilehash: af2855f18f07f200c28332965f3371117a61fba9
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66313275"
---
# <a name="adding-a-sub-domain"></a>Hinzufügen einer Unterdomäne

Unterdomänen können demselben oder einem anderen Mandanten als der übergeordneten Domäne hinzugefügt werden. In beiden Fällen müssen Sie Ihre eigenen DNS-Einstellungen auf der Website Ihrer Registrierungsstelle verwalten. Wenn Sie Zulassen, dass Microsoft Ihre DNS-Einstellungen mit NS-Einträgen verwaltet, oder wenn Sie die Domäne von Microsoft erworben haben, können Sie keine Unterdomänen hinzufügen, ohne diese zuerst zu ändern.

Fügen Sie zuerst die übergeordnete Domäne und dann die Unterdomäne hinzu. Wenn sich die Unterdomäne im selben Mandanten befindet, ist keine zusätzliche Überprüfung erforderlich. Wenn Sie die Unterdomäne einem separaten Mandanten hinzufügen, ist der DNS txt-Eintrag für die Besitzerüberprüfung erforderlich, bevor die Domäne und die zusätzlichen DNS-Einträge für die ausgewählten Dienste hinzugefügt werden.

- Um eine Domäne oder Unterdomäne hinzuzufügen, folgen [Sie dem Assistenten "Domäne hinzufügen"](https://admin.microsoft.com/Adminportal#/Domains/Wizard), oder fügen Sie die Domäne oder Unterdomäne manuell hinzu, indem Sie zu **"** > **Domänen** > **hinzufügen**" wechseln.

Falls erforderlich:

- Um zu ändern, wer Ihre DNS-Einstellungen für eine vorhandene Domäne verwaltet, wechseln Sie zu **"Domäneneinstellungen"** > [**, aktivieren**](https://admin.microsoft.com/Adminportal/Home#/Domains) Sie das Kontrollkästchen neben der Domäne, und wählen Sie dann **"DNS verwalten"** aus. Wählen Sie im Assistenten Ihre **eigenen DNS-Einträge hinzufügen aus,** und schließen Sie den Assistenten ab.
- Um einer von Microsoft erworbenen Domäne Unterdomänen hinzuzufügen, übertragen Sie die Domäne zuerst an eine andere Registrierungsstelle, und nehmen Sie dann die oben aufgeführte Änderung vor, um Ihre eigenen DNS-Einträge zu verwalten. Anweisungen finden Sie unter [Übertragen einer Domäne von Microsoft auf einen anderen Host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Wenn sie eine Fehlermeldung erhalten, dass Ihre Domäne bereits von anderen Mitgliedern oder Personen in Ihrer Organisation verwendet wird, müssen Sie zuerst dieses nicht verwaltete Konto übernehmen, bevor Sie die Domäne verwenden. Anweisungen hierzu finden [Sie unter Übernehmen eines nicht verwalteten Verzeichnisses als Administrator in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
