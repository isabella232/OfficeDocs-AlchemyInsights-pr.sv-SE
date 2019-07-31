---
title: Problem att logga in på Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938360"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="56aee-102">Fastställande av meddelandet ”datorns betrodda Platform module inte fungerar som det ska” apps Office</span><span class="sxs-lookup"><span data-stu-id="56aee-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="56aee-103">Försök med följande om du vill åtgärda det här felet:</span><span class="sxs-lookup"><span data-stu-id="56aee-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="56aee-104">Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="56aee-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="56aee-105">[Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.</span><span class="sxs-lookup"><span data-stu-id="56aee-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="56aee-106">**Observera:** Registersökvägar 2016 för Office har ändrats till 16,0.</span><span class="sxs-lookup"><span data-stu-id="56aee-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="56aee-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="56aee-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="56aee-108">Försök åtgärda fel Trusted Platform Module (TPM) [användaren återställningsprocessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .</span><span class="sxs-lookup"><span data-stu-id="56aee-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="56aee-109">Ange EnableADAL = 0 med hjälp av följande steg:</span><span class="sxs-lookup"><span data-stu-id="56aee-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="56aee-110">Högerklicka på Start, Välj **Kör**, Skriv **regedit**och klicka sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="56aee-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="56aee-111">Välj **Ja** så att Registereditorn för att göra ändringar i din enhet.</span><span class="sxs-lookup"><span data-stu-id="56aee-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="56aee-112">I Registereditorn kan du lägga till DWORD-värdet **EnableADAL** med en inställning på **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="56aee-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="56aee-113">Mer information finns i [anslutning problem i logga in efter uppdatering till Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="56aee-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>