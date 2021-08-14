---
title: Överföringstjänster – flytta alla RDFE-tjänster till en annan prenumeration
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940111"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Överföringstjänster – flytta alla RDFE-tjänster till en annan prenumeration

**Flytta resurser**

Azure-resurser kan flyttas till en annan Azure-prenumeration eller resursgrupp under samma prenumeration med hjälp av Azure-portalen, Azure PowerShell, Azure CLI eller REST API för att flytta resurser.

Innan du kan flytta resurser kan du se:

- [Checklista innan resurser flyttas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Tjänster som kan flyttas](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Så här verifierar du flytten](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Flytta vägledning för tjänster](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Om du vill flytta befintliga resurser till en annan resursgrupp eller prenumeration kan du använda:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST-API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Självstudiekurs: [Flytta Azure-resurser till en annan resursgrupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Felsöka fel med Azure Resource Manager**

I artiklarna nedan finns information om några vanliga Azure-distributionsfel och information om hur du löser dem. Om du inte hittar felkoden för distributionsfelet kan du gå till [Hitta felkod](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Felsöka distributionsfel](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Felsöka flytt av Azure-resurser till ny resursgrupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Observera att om du vill uppgradera din Azure-prenumeration, till exempel byta från kostnadsfri till betalning efter behov, måste du konvertera din prenumeration.

- Om du vill uppgradera en kostnadsfri utvärderingsversion kan du läsa Uppgradera din kostnadsfria utvärderingsversion eller [Microsoft Imagine Azure-prenumeration till Betala per användning.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Om du vill ändra ett konto med betalning efter användning kan du läsa Ändra [din Azure-prenumeration](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)med betalning efter användning till ett annat erbjudande.

**Så här lägger du till eller kopplar en Azure-prenumeration Azure Active Directory klientorganisationen:**

1. Logga in och välj den prenumeration du vill använda från sidan [Prenumerationer i Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Välj **Ändra katalog**.
3. Granska alla varningar som visas och välj sedan **Ändra**.
4. Katalogen ändras för prenumerationen och du får ett meddelande om detta.
5. Använd *Katalogväxeln* för att gå till den nya katalogen. Det kan ta upp till 10 minuter för allt att visas korrekt.

**Rekommenderade dokument**

- [Överföra ägarskapet för en Azure-prenumeration](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Flytta resurser till en ny resursgrupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Hantera resurser med Hjälp av Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
