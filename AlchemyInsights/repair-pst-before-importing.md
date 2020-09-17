---
title: Reparera. PST-fil före import
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799114"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="bb7ec-102">Reparera. PST-fil före import</span><span class="sxs-lookup"><span data-stu-id="bb7ec-102">Repair .pst file before importing</span></span>

<span data-ttu-id="bb7ec-103">Innan du importerar en PST-fil i Outlook bör du kontrol lera att filen inte är skadad genom att reparera filen:</span><span class="sxs-lookup"><span data-stu-id="bb7ec-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="bb7ec-104">Avsluta Outlook.</span><span class="sxs-lookup"><span data-stu-id="bb7ec-104">Exit Outlook.</span></span>

2. <span data-ttu-id="bb7ec-105">Hitta och kör `Scanpst.exe` i mappen Office-program (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> eller c:\Program\Microsoft Office\root\Office \<Version\> ).</span><span class="sxs-lookup"><span data-stu-id="bb7ec-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="bb7ec-106">I **reparations verktyget för Inkorgen för Microsoft Outlook**klickar du på **Bläddra** och letar reda på PST-filen (till exempel i C:\Users \\<username \> \AppData\Local\Microsoft\Outlook).</span><span class="sxs-lookup"><span data-stu-id="bb7ec-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="bb7ec-107">Välj PST-filen och klicka på **Öppna**.</span><span class="sxs-lookup"><span data-stu-id="bb7ec-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="bb7ec-108">Klicka på **Start** för att starta genomsökningen.</span><span class="sxs-lookup"><span data-stu-id="bb7ec-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="bb7ec-109">Om fel hittas i filen klickar du på **Reparera**och sedan på **OK** när reparationen är klar.</span><span class="sxs-lookup"><span data-stu-id="bb7ec-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="bb7ec-110">Försök importera PST-filen i Outlook igen.</span><span class="sxs-lookup"><span data-stu-id="bb7ec-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="bb7ec-111">Mer information finns i [Reparera Outlook-datafiler](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) och [åtgärda problem med att importera en Outlook. PST-fil](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="bb7ec-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
