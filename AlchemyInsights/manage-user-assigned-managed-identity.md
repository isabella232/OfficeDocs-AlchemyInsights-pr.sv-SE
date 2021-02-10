---
title: Hantera en användar kopplad hanterad identitet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177778"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="532ef-102">Hantera en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="532ef-103">Hanteringen av en användar tilldelad hanterad identitet omfattar:</span><span class="sxs-lookup"><span data-stu-id="532ef-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="532ef-104">Tilldela roller till en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="532ef-105">Ta bort en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="532ef-106">Visa en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="532ef-107">Mer information om de uppgifter som nämns ovan finns i följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="532ef-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="532ef-108">[Så här skapar du en användar tilldelad hanterad identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – för att tilldela roller till en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="532ef-109">[Så här tar du bort en användar kopplad hanterad identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – för att ta bort en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="532ef-110">[Så här visar du en användar kopplad hanterad identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – för att visa en användar kopplad hanterad identitet</span><span class="sxs-lookup"><span data-stu-id="532ef-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="532ef-111">Kontrollera om du har **rolltilldelningen Hanterad identitetsdeltagare.**</span><span class="sxs-lookup"><span data-stu-id="532ef-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="532ef-112">Den rolltilldelningen krävs för att skapa/ta bort användartilldelningar av hanterade identiteter.</span><span class="sxs-lookup"><span data-stu-id="532ef-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
