---
title: Använda metodtips för avancerade sökfrågor
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749550"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="61870-102">Använda metodtips för avancerade sökfrågor</span><span class="sxs-lookup"><span data-stu-id="61870-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="61870-103">Använd de här metodtipsen för att få resultat snabbare och undvika tidsgränser när du kör komplexa frågor:</span><span class="sxs-lookup"><span data-stu-id="61870-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="61870-104">När du försöker med nya frågor ska du alltid använda en gräns, för att undvika att få extremt stora resultatuppsättningar.</span><span class="sxs-lookup"><span data-stu-id="61870-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="61870-105">Använd också `count` för att göra en första bedömning av storleken på resultatuppsättningen.</span><span class="sxs-lookup"><span data-stu-id="61870-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="61870-106">Använd tidsfilter först.</span><span class="sxs-lookup"><span data-stu-id="61870-106">Use time filters first.</span></span> <span data-ttu-id="61870-107">Under idealiska tider bör du begränsa dina frågor till sju dagar.</span><span class="sxs-lookup"><span data-stu-id="61870-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="61870-108">I början av en fråga, direkt efter tidsfiltret, lägger du till de filter som förväntas ta bort de flesta data.</span><span class="sxs-lookup"><span data-stu-id="61870-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="61870-109">När du söker efter fullständiga token ska du använda `has` operatorn i stället för `contains` .</span><span class="sxs-lookup"><span data-stu-id="61870-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="61870-110">Kör en sökning på en specifik kolumn i stället för i alla kolumner.</span><span class="sxs-lookup"><span data-stu-id="61870-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="61870-111">När du sammanfogar tabeller ska du först ange tabellen med färre rader.</span><span class="sxs-lookup"><span data-stu-id="61870-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="61870-112">`project` endast de kolumner som behövs i tabellerna som du har anslutit till.</span><span class="sxs-lookup"><span data-stu-id="61870-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="61870-113">Mer information finns i Avancerad [frågedesign.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="61870-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
