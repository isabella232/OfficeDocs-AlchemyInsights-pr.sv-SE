---
title: Nätverkskommunikation
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799582"
---
# <a name="network-migration"></a><span data-ttu-id="42d39-102">Nätverkskommunikation</span><span class="sxs-lookup"><span data-stu-id="42d39-102">Network Migration</span></span>

<span data-ttu-id="42d39-103">Din O365-klient organisation är eventuellt kopplad till flera Yammer-nätverk i en 1 klient organisation: många nätverks konfiguration.</span><span class="sxs-lookup"><span data-stu-id="42d39-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="42d39-104">Från och med den 16 oktober 2018 stöder Yammer inte längre flera Yammer-nätverk som är associerade med en klient organisation.</span><span class="sxs-lookup"><span data-stu-id="42d39-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="42d39-105">Du kan göra en nätverks migrering för att komma till en Preferred 1:1-konfiguration.</span><span class="sxs-lookup"><span data-stu-id="42d39-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="42d39-106">Om du vill visa en lista över de nätverk som är kopplade till din klient organisation, loggar du in på Yammer som global administratör och bläddrar till **nätverks administratör**och sedan på **nätverkskommunikation**.</span><span class="sxs-lookup"><span data-stu-id="42d39-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="42d39-107">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="42d39-107">Choose **Next**.</span></span>

- <span data-ttu-id="42d39-108">Om flera nätverk visas i steg 2 av 3 har du flera Yammer-nätverk kopplade till din O365-klient organisation.</span><span class="sxs-lookup"><span data-stu-id="42d39-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="42d39-109">Om du vill korrigera konfigurationen för en 1:1-konfiguration fortsätter du med verktyget för nätverksdiagnostik.</span><span class="sxs-lookup"><span data-stu-id="42d39-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="42d39-110">Mer information om nätverksautentisering finns i [nätverks migrering: konsolidera flera Yammer-nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="42d39-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="42d39-111">Observera:</span><span class="sxs-lookup"><span data-stu-id="42d39-111">Please Note:</span></span>
  
- <span data-ttu-id="42d39-112">**En nätverks migrering migrerar bara aktiva och väntande användare.**</span><span class="sxs-lookup"><span data-stu-id="42d39-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="42d39-113">Tillsammans med aktiva användare migreras användarnas information, till exempel namn och profil bild.</span><span class="sxs-lookup"><span data-stu-id="42d39-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="42d39-114">Allt nätverks innehåll, inklusive grupper, migreras inte.</span><span class="sxs-lookup"><span data-stu-id="42d39-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="42d39-115">**Det går inte att byta nätverks överföring.**</span><span class="sxs-lookup"><span data-stu-id="42d39-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="42d39-116">Du kommer inte att kunna komma åt ditt dotter bolag och dess innehåll efter migreringen.</span><span class="sxs-lookup"><span data-stu-id="42d39-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="42d39-117">Så innan du funderar på att migrera kan du planera omsorgsfullt.</span><span class="sxs-lookup"><span data-stu-id="42d39-117">So before you consider a migration, you want to plan carefully.</span></span>
