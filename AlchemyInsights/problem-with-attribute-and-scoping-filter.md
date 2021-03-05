---
title: Problem med attribut- och scopingfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482923"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem med attribut- och scopingfilter

**Problem med upn-värden i konflikt**

Arbetsdagar till AD-användaretablering – arbetsdagar till AD-användaretablering visar **felmeddelandet HybridSynkroniseringActiveDirectoryUserPrincipalNameNotUnique.** Åtgärden misslyckades eftersom UPN-värde som angetts för tillägg/ändring inte är unikt för hela skogen. Felinformation: **CONSTRAINT_ATT_TYPE – userPrincipalName.**

Värdet **för userPrincipalName** som Workday-kopplingen försöker ange när AD-användarkontot skapas finns redan i AD-måldomänen. Detta antyder att antingen (1) användaren redan finns och att den matchande ID-kontrollen misslyckades för användaren eller (2) genererade UPN-regeln ett värde i konflikt.

Här är de föreslagna lösningsstegen:

Om det inte gick att länka arbetsdagar-kontot till Active Directory-kontot och det inte gick att länka det matchande ID-attributet (normalt anställnings-ID) i både Arbetsdagar och AD om det redan finns en exakt matchning. Om de inte har någon matchning är det ett dataproblem som måste åtgärdas. Om anställnings-ID:t i Arbetsdagar till exempel är 001052 och i AD är det 1052 går det inte att länka de två kontona och försöker skapa en användare som redan finns. Lösningen i det här fallet är att ändra värdet för **Anställnings-ID** i AD så att inledande nollor inkluderas så att det blir 001052.
Om UPN-genererande uttryck inte genererar ett unikt värde bör du överväga att använda avdupliceringsfunktionen **SelectUniqueValue** för att generera ett unikt värde varje gång.

**Arbetsdagar till AD-användaretablering anger inte managerattributvärdet för AD-användarkontot**

Arbetsdagar till AD-jobbet för användaretablering anger inte **managerattributvärdet** för AD-användarkonton. Det finns två möjliga scenarier när det här beteendet visas:

1. Chefen under Arbetsdagar kan inte matchas med ett motsvarande AD-användarkonto eftersom chefen inte omfattas.
2. I ett **scenario med flera AD-domäner** finns inte chefen i Arbetsdag i samma domän som användaren.

Prova följande för att lösa problemet:

1. Om du har definierat omfattningsfilter kontrollerar du först om chefen ingår i omfattningen och att den uppfyller omfattningssatsen. Om chefen inte uppfyller omfattningen för filtret ändrar du filtret så att chefen också omfattas av etableringsåtgärden.
2. Om du har flera AD-domäner har kopplingen en känd begränsning av att det inte går att lösa referenser till flera domänhanterare.

Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













