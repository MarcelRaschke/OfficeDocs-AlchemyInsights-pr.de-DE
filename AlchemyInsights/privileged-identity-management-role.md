---
title: Privileged Identity Management Rolle
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 1d53573074839172a227be3397870c593ffa3e11
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66265600"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)-Rolle

**Berechtigungen werden nach der Aktivierung einer Rolle nicht gewährt**

Wenn Sie eine Rolle in Azure AD Privileged Identity Management (PIM) aktivieren, wird die Aktivierung möglicherweise nicht sofort an alle Portale weitergegeben, für die die privilegierte Rolle erforderlich ist. Manchmal kann die Webzwischenspeicherung in einem Portal dazu führen, dass die Änderung nicht sofort wirksam wird, auch wenn die Änderung weitergegeben wird.

Wenn die Aktivierung verzögert ist, führen Sie die folgenden Schritte aus:

1. Melden Sie sich vom Azure-Portal ab, und melden Sie sich dann wieder an. Wenn Sie eine Azure AD-Rolle oder eine Azure-Ressourcenrolle aktivieren, werden die Phasen Ihrer Aktivierung angezeigt. Sobald alle Phasen abgeschlossen sind, wird der Link "Abmelden" angezeigt. Sie können diesen Link verwenden, um sich abzumelden. Dies löst die meisten Fälle für Aktivierungsverzögerungen.
2. Stellen Sie in PIM sicher, dass Sie als Mitglied der Rolle aufgeführt sind.
3. Wenn Sie die Exchange-Administratorrolle aktivieren, stellen Sie sicher, dass Sie sich abmelden und wieder anmelden. Wenn das Problem weiterhin besteht, öffnen Sie ein Supportticket, und lösen Sie es als Problem aus. Wenn Sie Ihre Exchange-Administratorrolle für den Zugriff auf das Security and Compliance Center verwenden, lesen Sie den nächsten Schritt.
4. Wenn Sie eine Rolle für den Zugriff auf das Security and Compliance Center aktivieren oder die SharePoint-Administratorrolle aktivieren, kommt es zu einer Aktivierungsverzögerung von einigen Minuten bis zu einigen Stunden. Dies ist ein bekanntes Problem, und wir arbeiten aktiv mit diesen Teams zusammen, um dieses Problem so schnell wie möglich zu beheben.

Weitere Informationen finden Sie unter:

- [Aktivieren meiner Azure AD-Rollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivieren meiner Azure-Ressourcenrollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Berechtigungen werden nicht entfernt, nachdem eine Rolle deaktiviert wurde oder die Rollenaktivierung abläuft.**

Wenn Sie eine Rolle in Azure AD Privileged Identity Management deaktivieren oder wenn ein Aktivierungszeitraum für Rollen abläuft, kann es zu einer Verzögerung kommen, auf die Sie weiterhin Zugriff haben.

Wenn die Deaktivierung verzögert wird, führen Sie die folgenden Schritte aus:

1. Wenn Sie die Exchange-Administratorrolle deaktivieren oder der Aktivierungszeitraum für die Rolle abläuft und Sie eine erhebliche Verzögerung bemerken, bevor die Berechtigungen entfernt werden, öffnen Sie ein Supportticket, und bitten Sie Ihren Supporttechniker, Ihnen bei der Datei eines Tickets mit dem PAM-Team (Privileged Access Management) in Office zu diesem Problem zu helfen.
2. Wenn der Aktivierungszeitraum abgelaufen ist, Die Browsersitzung aber weiterhin geöffnet ist, schließen Sie Ihren Browser. Sie können die Rolle weiterhin verwenden, bis Sie diese Sitzung schließen. Dies ist ein bekanntes Problem, und wir untersuchen einen potenziellen Fix, um jede Sitzung aktiv zu widerrufen, sobald die Aktivierung abgelaufen ist.

Wenn Sich Ihre Verzögerung von diesen beiden Szenarien unterscheidet, öffnen Sie bitte ein Supportticket.
