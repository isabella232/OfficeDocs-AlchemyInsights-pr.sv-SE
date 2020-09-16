---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745148"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Åtgärda 0x8004de40-fel i OneDrive

Om du får ett 0x8004de40-fel med OneDrive:

- Starta om datorn när den är ansluten till din Acitve-katalog.
- Om det inte går att åtgärda problemet kan du koppla från och återansluta till enheten från Azure AD. 

**Obs!** du bör vara på företagets nätverk när du utför de här stegen. Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser). 

- Öppna en upphöjd kommando tolk. 
- Öppna en upphöjd kommando tolk genom att klicka på **Start**, högerklicka på **kommando tolken**och klicka sedan på **Kör som administratör**.
- Skriv *dsregcmd/Leave* och tryck på **RETUR**.
- När du är klar skriver du *dsregcmd/Join* och trycker på **RETUR**.
- När du är klar stänger du kommando tolken.
- Starta om datorn och logga in på OneDrive.