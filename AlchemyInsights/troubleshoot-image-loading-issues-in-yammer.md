---
title: Felsöka problem med inläsning av bilder i Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148300"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="65dde-102">Felsöka problem med inläsning av bilder i Yammer</span><span class="sxs-lookup"><span data-stu-id="65dde-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="65dde-103">När det uppstår problem med foton och förhandsgranskningar av filer i Yammer felsöker du genom att kontrollera om problemet uppstår för alla användare, om det uppstår på mobila enheter och om det kan reproduceras när den bifogade filen laddas upp.</span><span class="sxs-lookup"><span data-stu-id="65dde-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="65dde-104">**Problem med profilfoto**</span><span class="sxs-lookup"><span data-stu-id="65dde-104">**Profile photo issues**</span></span>  

<span data-ttu-id="65dde-105">Om slutanvändare loggar in på Yammer via Microsoft 365 måste de ändra sin profil, inklusive sitt profilfoto.</span><span class="sxs-lookup"><span data-stu-id="65dde-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="65dde-106">Om användare inte har rätt att göra profiluppdateringar kan en administratör göra uppdateringen för användaren.</span><span class="sxs-lookup"><span data-stu-id="65dde-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="65dde-107">Mer information finns i [Visa och uppdatera din profil i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="65dde-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="65dde-108">Information om profilredigering, inklusive profilfoton, finns i [Ändra min Yammer-profil och mina inställningar](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="65dde-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="65dde-109">Uppdaterade profilfoton synkroniseras på ett annat sätt än profilattribut.</span><span class="sxs-lookup"><span data-stu-id="65dde-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="65dde-110">Användare måste logga in för att initiera en synkronisering av deras profilfoto.</span><span class="sxs-lookup"><span data-stu-id="65dde-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="65dde-111">Mer information finns i [användarprofilbilder som uppdaterats från Office 365 till Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="65dde-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="65dde-112">Information om användarlivscykeln för Yammer finns i [Hantera Yammer-användare under hela livscykeln från Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="65dde-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="65dde-113">Mer information om hur synkronisering av profilbilder fungerar i Microsoft 365 finns [i Information om synkronisering av profilbilder i Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="65dde-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="65dde-114">**Dokumentförhandsgranskningar och problem med miniatyrbilden**</span><span class="sxs-lookup"><span data-stu-id="65dde-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="65dde-115">När filer eller bilder publiceras i Yammer kanske förhandsgranskningar inte visas på grund av:</span><span class="sxs-lookup"><span data-stu-id="65dde-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="65dde-116">Filen är skadad och kan inte bearbetas.</span><span class="sxs-lookup"><span data-stu-id="65dde-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="65dde-117">Filen har inte nyligen överförts till SharePoint Online, eller Yammer har ogiltiga metadata av andra skäl.</span><span class="sxs-lookup"><span data-stu-id="65dde-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="65dde-118">Webbadresser som krävs för att läsa in förhandsgranskningsbilderna blockeras.</span><span class="sxs-lookup"><span data-stu-id="65dde-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="65dde-119">Förhandsgranskningen av filen togs bort av användaren innan den bokfördes.</span><span class="sxs-lookup"><span data-stu-id="65dde-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="65dde-120">Ett serviceproblem förhindrade att en förhandsgranskning genererades.</span><span class="sxs-lookup"><span data-stu-id="65dde-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="65dde-121">**Anm.)** Förhandsgranskningar för länkar och filuppladdningar kan bete sig annorlunda.</span><span class="sxs-lookup"><span data-stu-id="65dde-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="65dde-122">Länkar till filer på internet eller länkar som kräver ytterligare autentisering kanske inte visas korrekt.</span><span class="sxs-lookup"><span data-stu-id="65dde-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="65dde-123">Mer information finns i [Bifoga en fil eller bild i ett Yammer-meddelande](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="65dde-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 