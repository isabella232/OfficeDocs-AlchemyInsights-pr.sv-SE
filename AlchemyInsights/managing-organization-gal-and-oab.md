---
title: Hantera organisationens globala adresslista och offlineadressbok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794850"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="f51de-102">Hantera organisationens globala adresslista och offlineadressbok</span><span class="sxs-lookup"><span data-stu-id="f51de-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="f51de-103">En global adresslista är en lista över e-postaktiverade objekt (alla typer av mottagare som kan ta emot e-post) i organisationen.</span><span class="sxs-lookup"><span data-stu-id="f51de-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="f51de-104">En global adresslista skapas automatiskt i alla organisationer.</span><span class="sxs-lookup"><span data-stu-id="f51de-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="f51de-105">Du kan skapa flera globala adresslistor för att separera användare efter organisation eller plats, men en enskild användare kan bara se och använda en global adresslista i taget.</span><span class="sxs-lookup"><span data-stu-id="f51de-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="f51de-106">Vissa e-postklienter, till exempel Outlook för Windows, laddar ned den globala adresslistan för offlineanvändning.</span><span class="sxs-lookup"><span data-stu-id="f51de-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="f51de-107">Det kallas offlineadressbok.</span><span class="sxs-lookup"><span data-stu-id="f51de-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="f51de-108">Exchange Online uppdateras en offlineadressbok bara en gång var 8:e timme och sedan måste klienterna ladda ned den för att uppdatera den lokala kopian av offlineadressboken.</span><span class="sxs-lookup"><span data-stu-id="f51de-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="f51de-109">Alla mottagarändringar måste först synas i den globala adresslistan för att senare hamna i offlineadressboken.</span><span class="sxs-lookup"><span data-stu-id="f51de-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="f51de-110">Här är några vanliga procedurer för global adresslista och offlineadressbok:</span><span class="sxs-lookup"><span data-stu-id="f51de-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="f51de-111">Av olika anledningar kanske du vill dölja vissa objekt i den globala adresslistan.</span><span class="sxs-lookup"><span data-stu-id="f51de-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="f51de-112">Se [Dölja mottagare i adresslistor](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="f51de-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="f51de-113">Om du behöver ge specifika grupper anpassade vyer av organisationens globala adresslista kan du läsa artikeln om [adressboksprinciper i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="f51de-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="f51de-114">[Skapa en global adresslista i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) och om du vill lära dig hur du arbetar med behörigheter för globala adresslistor läser du artikeln om [adresslistor i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="f51de-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="f51de-115">Obs! Om du vill skapa nya globala adresslistor kanske du även vill skapa en ny offlineadressbok.</span><span class="sxs-lookup"><span data-stu-id="f51de-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="f51de-116">Se artikeln om [procedurer för offlineadressböcker](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="f51de-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
