---
title: Lösa problem med okända användare i Teams-chatt
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
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807775"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="97b72-102">Lösa problem med "okänd användare" i Teams-chatten</span><span class="sxs-lookup"><span data-stu-id="97b72-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="97b72-103">Ibland visas en borttagen användare som "okänd användare".</span><span class="sxs-lookup"><span data-stu-id="97b72-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="97b72-104">Detta är ett [känt problem](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span><span class="sxs-lookup"><span data-stu-id="97b72-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="97b72-105">Om du ser användarna bestående av "okända användare" i Teams-chattar kan du försöka med att rensa cacheminnet:</span><span class="sxs-lookup"><span data-stu-id="97b72-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="97b72-106">Högerklicka på Team ikonen i aktivitets fältet.</span><span class="sxs-lookup"><span data-stu-id="97b72-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="97b72-107">Klicka på  **Avsluta** .</span><span class="sxs-lookup"><span data-stu-id="97b72-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="97b72-108">Bläddra till%appdata%\Microsoft\teams\-mappen på datorn och ta bort alla filer i den katalogen.</span><span class="sxs-lookup"><span data-stu-id="97b72-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="97b72-109">Du kan förhindra att anonyma användare ansluter till möten genom att se till att de väntar i lobbyn.</span><span class="sxs-lookup"><span data-stu-id="97b72-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="97b72-110">Mer information finns i [ändra deltagar inställningar för ett Teams-möte](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span><span class="sxs-lookup"><span data-stu-id="97b72-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
