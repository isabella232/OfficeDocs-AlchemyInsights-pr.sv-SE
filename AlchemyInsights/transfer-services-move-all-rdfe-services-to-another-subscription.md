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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="ca4ac-102">Överförings tjänster-flytta alla RDFE-tjänster till en annan prenumeration</span><span class="sxs-lookup"><span data-stu-id="ca4ac-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="ca4ac-103">**Flytta resurser**</span><span class="sxs-lookup"><span data-stu-id="ca4ac-103">**Move resources**</span></span>

<span data-ttu-id="ca4ac-104">Azure-resurser kan flyttas till antingen en annan Azure-prenumeration eller resurs grupp under samma abonnemang med Azure Portal, Azure PowerShell, Azure CLI eller REST API för att flytta resurser.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="ca4ac-105">Innan du kan flytta resurser, se:</span><span class="sxs-lookup"><span data-stu-id="ca4ac-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="ca4ac-106">Check lista innan du flyttar resurser</span><span class="sxs-lookup"><span data-stu-id="ca4ac-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="ca4ac-107">Tjänster som kan flyttas</span><span class="sxs-lookup"><span data-stu-id="ca4ac-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="ca4ac-108">Verifiera flytten</span><span class="sxs-lookup"><span data-stu-id="ca4ac-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="ca4ac-109">Flytta vägledning för tjänster</span><span class="sxs-lookup"><span data-stu-id="ca4ac-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="ca4ac-110">Om du vill flytta befintliga resurser till en annan resurs grupp eller prenumeration kan du använda:</span><span class="sxs-lookup"><span data-stu-id="ca4ac-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="ca4ac-111">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ca4ac-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="ca4ac-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ca4ac-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="ca4ac-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ca4ac-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="ca4ac-114">REST API</span><span class="sxs-lookup"><span data-stu-id="ca4ac-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="ca4ac-115">Själv studie kurs: [Flytta Azure-resurser till en annan resurs grupp eller prenumeration](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="ca4ac-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="ca4ac-116">**Felsöka fel med Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="ca4ac-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="ca4ac-117">Läs artiklarna nedan för att få mer information om vanliga Azure-distributionspaket och hur du löser dem.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="ca4ac-118">Om du inte hittar felkoden för distributions felet, se [find felkod](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="ca4ac-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="ca4ac-119">Felsöka distributions fel</span><span class="sxs-lookup"><span data-stu-id="ca4ac-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="ca4ac-120">Felsöka flytt av Azure-resurser till en ny resurs grupp eller prenumeration</span><span class="sxs-lookup"><span data-stu-id="ca4ac-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="ca4ac-121">Observera att om du vill uppgradera ditt Azure-abonnemang, till exempel att byta från gratis för att betala allt eftersom, måste du konvertera prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="ca4ac-122">Om du vill uppgradera en kostnads fri utvärderings version kan [du läsa uppgradera din gratis prov period eller Microsoft Föreställ dig Azure-abonnemang för att betala allt eftersom](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="ca4ac-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="ca4ac-123">Information om hur du ändrar ett konto för betala allt eftersom finns i [ändra ditt Azure betala-allteftersom-abonnemang till ett annat erbjudande](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="ca4ac-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="ca4ac-124">**Lägga till eller koppla ett Azure-abonnemang till din Azure Active Directory-klient organisation:**</span><span class="sxs-lookup"><span data-stu-id="ca4ac-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="ca4ac-125">Logga in och välj den prenumeration du vill använda från [sidan prenumerationer i Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="ca4ac-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="ca4ac-126">Välj **ändra katalog**.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="ca4ac-127">Granska eventuella varningar som visas och välj sedan **ändra**.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="ca4ac-128">Katalogen ändras för abonnemanget och du får ett meddelande om att meddelandet lyckades.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="ca4ac-129">Gå till den nya katalogen med *katalog* växlaren.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="ca4ac-130">Det kan ta upp till 10 minuter innan allting visas korrekt.</span><span class="sxs-lookup"><span data-stu-id="ca4ac-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="ca4ac-131">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="ca4ac-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="ca4ac-132">Överföra ägande av en Azure-prenumeration</span><span class="sxs-lookup"><span data-stu-id="ca4ac-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="ca4ac-133">Flytta resurser till en ny resurs grupp eller prenumeration</span><span class="sxs-lookup"><span data-stu-id="ca4ac-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="ca4ac-134">Hantera resurser med Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ca4ac-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
