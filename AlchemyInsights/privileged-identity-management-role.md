---
title: Rolle "Privileged Identity Management"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: ba12061a866063fe7cd8a64575cf19fb6a38cb2c
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63305569"
---
# <a name="privileged-identity-managementpim-role"></a>rolle Privileged Identity Management(PIM)

**Berechtigungen werden nach der Aktivierung einer Rolle nicht gewährt**

Wenn Sie eine Rolle in Azure AD Privileged Identity Management (PIM) aktivieren, wird die Aktivierung möglicherweise nicht sofort an alle Portale verteilt, die die privilegierte Rolle erfordern. Manchmal kann die Webzwischenspeicherung in einem Portal auch dann, wenn die Änderung weitergegeben wird, dazu führen, dass die Änderung nicht sofort wirksam wird.

Wenn die Aktivierung verzögert wird, führen Sie die folgenden Schritte aus:

1. Melden Sie sich vom Azure-Portal ab, und melden Sie sich dann wieder an. Wenn Sie eine Azure AD Rolle oder eine Azure-Ressourcenrolle aktivieren, sehen Sie die Phasen Ihrer Aktivierung. Sobald alle Phasen abgeschlossen sind, wird der Link "Abmelden" angezeigt. Über diesen Link können Sie sich abmelden. Dadurch werden die meisten Fälle von Aktivierungsverzögerung behoben.
2. Überprüfen Sie in PIM, ob Sie als Mitglied der Rolle aufgeführt sind.
3. Wenn Sie die Exchange Administratorrolle aktivieren, stellen Sie sicher, dass Sie sich abmelden und wieder anmelden. Wenn das Problem weiterhin besteht, öffnen Sie ein Supportticket, und lösen Sie es als Problem aus. Wenn Sie Ihre Exchange Administratorrolle für den Zugriff auf das Security and Compliance Center verwenden, lesen Sie den nächsten Schritt.
4. Wenn Sie eine Rolle aktivieren, um auf das Security and Compliance Center zuzugreifen, oder wenn Sie die SharePoint Administratorrolle aktivieren, tritt eine Aktivierungsverzögerung von einigen Minuten bis zu einigen Stunden auf. Dies ist ein bekanntes Problem, und wir arbeiten aktiv mit diesen Teams zusammen, um dieses Problem so schnell wie möglich zu beheben.

Weitere Informationen finden Sie unter:

- [Aktivieren meiner Azure AD Rollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivieren meiner Azure-Ressourcenrollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Berechtigungen werden nicht entfernt, nachdem eine Rolle deaktiviert wurde oder die Rollenaktivierung abläuft.**

Wenn Sie eine Rolle in Azure AD Privileged Identity Management deaktivieren oder wenn ein Aktivierungszeitraum für Rollen abläuft, kann es zu einer Verzögerung kommen, wenn Sie weiterhin Zugriff haben.

Wenn die Deaktivierung verzögert wird, führen Sie die folgenden Schritte aus:

1. Wenn Sie die Exchange Administratorrolle deaktivieren oder der Aktivierungszeitraum der Rolle abläuft und Sie eine erhebliche Verzögerung bemerken, bevor die Berechtigungen entfernt werden, öffnen Sie ein Supportticket, und weisen Sie Ihren Supporttechniker an, Ihnen zu helfen, innerhalb Office zu diesem Problem ein Ticket beim Pam-Team (Privileged Access Management) zu beantragen.
2. Wenn der Aktivierungszeitraum abgelaufen ist, Sie die Browsersitzung aber noch geöffnet haben, schließen Sie Ihren Browser. Sie können die Rolle weiterhin verwenden, bis Sie diese Sitzung schließen. Dies ist ein bekanntes Problem, und wir sehen uns einen potenziellen Fix an, um jede Sitzung aktiv zu widerrufen, sobald die Aktivierung abgelaufen ist.

Wenn sich Ihre Verzögerung von diesen beiden Szenarien unterscheidet, öffnen Sie bitte ein Supportticket.
