---
title: Överförings tjänster-flytta alla RDFE-tjänster till en annan prenumeration
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692178"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Överförings tjänster-flytta alla RDFE-tjänster till en annan prenumeration

**Flytta resurser**

Azure-resurser kan flyttas till antingen en annan Azure-prenumeration eller resurs grupp under samma abonnemang med Azure Portal, Azure PowerShell, Azure CLI eller REST API för att flytta resurser.

Innan du kan flytta resurser, se:

- [Check lista innan du flyttar resurser](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Tjänster som kan flyttas](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Verifiera flytten](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Flytta vägledning för tjänster](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Om du vill flytta befintliga resurser till en annan resurs grupp eller prenumeration kan du använda:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Själv studie kurs: [Flytta Azure-resurser till en annan resurs grupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Felsöka fel med Azure Resource Manager**

Läs artiklarna nedan för att få mer information om vanliga Azure-distributionspaket och hur du löser dem. Om du inte hittar felkoden för distributions felet, se [find felkod](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Felsöka distributions fel](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Felsöka flytt av Azure-resurser till en ny resurs grupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Observera att om du vill uppgradera ditt Azure-abonnemang, till exempel att byta från gratis för att betala allt eftersom, måste du konvertera prenumerationen.

- Om du vill uppgradera en kostnads fri utvärderings version kan [du läsa uppgradera din gratis prov period eller Microsoft Föreställ dig Azure-abonnemang för att betala allt eftersom](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Information om hur du ändrar ett konto för betala allt eftersom finns i [ändra ditt Azure betala-allteftersom-abonnemang till ett annat erbjudande](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Lägga till eller koppla ett Azure-abonnemang till din Azure Active Directory-klient organisation:**

1. Logga in och välj den prenumeration du vill använda från [sidan prenumerationer i Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Välj **ändra katalog**.
3. Granska eventuella varningar som visas och välj sedan **ändra**.
4. Katalogen ändras för abonnemanget och du får ett meddelande om att meddelandet lyckades.
5. Gå till den nya katalogen med *katalog* växlaren. Det kan ta upp till 10 minuter innan allting visas korrekt.

**Rekommenderade dokument**

- [Överföra ägande av en Azure-prenumeration](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Flytta resurser till en ny resurs grupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Hantera resurser med Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
