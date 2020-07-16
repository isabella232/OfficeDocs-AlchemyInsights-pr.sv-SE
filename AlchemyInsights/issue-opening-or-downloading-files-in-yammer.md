---
title: Problem med att öppna eller ladda ned filer i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148437"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="1bfcb-102">Problem med att öppna eller ladda ned filer i Yammer</span><span class="sxs-lookup"><span data-stu-id="1bfcb-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="1bfcb-103">Classic Yammer stöder flera alternativ för filuppladdningar till meddelanden och grupper.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="1bfcb-104">Beroende på nätverkskonfiguration, filer som standard lagring i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="1bfcb-105">Filväljaren i nya Yammer stöder ännu inte alla alternativ som finns i klassiska Yammer.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="1bfcb-106">En framtida uppdatering kommer att lägga till ytterligare funktioner.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-106">A future update will add additional features.</span></span> <span data-ttu-id="1bfcb-107">Mer information finns i [Bifoga en fil eller bild i ett Yammer-konversationsinlägg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="1bfcb-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="1bfcb-108">**Det går inte att öppna eller hämta en fil**</span><span class="sxs-lookup"><span data-stu-id="1bfcb-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="1bfcb-109">En fil kan överföras till Yammer men också länka till en fil i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="1bfcb-110">Om du vill felsöka måste du först bestämma platsen för filen.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="1bfcb-111">Om filen har överförts till Yammer har den en \*.yammer.com-URL.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="1bfcb-112">Kontrollera att nödvändiga webbadresser och IP-adresser är avblockerade.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="1bfcb-113">Mer information finns i blogginlägget [Använda hårdkodade IP-adresser för Yammer rekommenderas inte](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="1bfcb-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="1bfcb-114">Kontrollera om en användare som också är global administratör kan hämta filen.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="1bfcb-115">Om filen är privat kan du behöva använda privat innehållsläge.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="1bfcb-116">Mer information finns [i Övervaka privat innehåll i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="1bfcb-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="1bfcb-117">**Gäster och filer på Yammer-nätverksnivå i SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="1bfcb-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="1bfcb-118">[Gäster på nätverksnivå i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) använder inte Azure AD B2B och är interna för Yammer-tjänsten, så att de inte kan komma åt Yammer-filer som lagras i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="1bfcb-119">Skapa en extern AAD B2B-användare som kan komma åt dokumentbibliotek i SharePoint Online med hjälp av den identiteten.</span><span class="sxs-lookup"><span data-stu-id="1bfcb-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="1bfcb-120">Information om framtida Azure AD B2B-gästsupport i Yammer finns [i B2B-gästsupport (Business-to-business) i Yammer Preview – Kundvillkor och vanliga frågor](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)och svar .</span><span class="sxs-lookup"><span data-stu-id="1bfcb-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>