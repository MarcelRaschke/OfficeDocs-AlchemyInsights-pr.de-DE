---
title: 'Beheben von Microsoft 365-Apps: Die zugeordnete Meldung "Office-Lizenzen konnte nicht gefunden werden"'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001426"
- "3421"
ms.openlocfilehash: a16d0a147c6a56d36818ee9da7f6454e436d34e7
ms.sourcegitcommit: 8324c868c664bfdee6d5bb99ad8d41e9dd46d10f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66539018"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Beheben der Meldung "Zugeordnete Office-Lizenzen konnten nicht gefunden werden" in Microsoft 365-Apps

Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie Ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie den Internetzugriff auf Microsoft 365-Apps nicht blockieren. Siehe [Microsoft 365-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Entfernen Sie [die Office-Lizenz für den](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) betroffenen Benutzer, und weisen Sie sie erneut zu. 
3. Öffnen Sie eine Office-App, und [melden Sie](https://support.microsoft.com/office/sign-out-of-office-5a20dc11-47e9-4b6f-945d-478cb6d92071of) alle vorhandenen Benutzerkonten ab.
4. Wechseln Sie zu Windows-Einstellungen > **Konten** > **– E-Mail-& Konten**, und entfernen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos.
5. Wechseln Sie zu Windows-Einstellungen > **Konten** > **greifen auf Geschäfts-, Schul- oder Unikonten** zu, und trennen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos.
6. Setzen Sie den Office-Aktivierungsstatus zurück. [Anleitung](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Melden Sie sich](https://support.microsoft.com/office/about-accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) mit dem betroffenen Benutzerkonto an.

Weitere Lösungen zur Problembehandlung finden Sie [unter "Nicht lizenziertes Produkt" und Aktivierungsfehler in Office](https://support.microsoft.com/office/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).