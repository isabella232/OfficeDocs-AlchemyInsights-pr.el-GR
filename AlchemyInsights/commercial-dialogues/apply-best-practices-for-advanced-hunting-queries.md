---
title: Εφαρμογή βέλτιστων πρακτικών για σύνθετα ερωτήματα κυνηγιού
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
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746181"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="e7418-102">Εφαρμογή βέλτιστων πρακτικών για σύνθετα ερωτήματα κυνηγιού</span><span class="sxs-lookup"><span data-stu-id="e7418-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="e7418-103">Για να έχετε αποτελέσματα πιο γρήγορα και για να αποφύγετε χρονικά ορίου κατά την εκτέλεση σύνθετων ερωτημάτων, εφαρμόστε αυτές τις βέλτιστες πρακτικές:</span><span class="sxs-lookup"><span data-stu-id="e7418-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="e7418-104">Όταν προσπαθείτε νέα ερωτήματα, χρησιμοποιείτε πάντα ένα όριο, για να αποφύγετε τη λήψη εξαιρετικά μεγάλων συνόλων αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="e7418-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="e7418-105">Επίσης, χρησιμοποιήστε `count` το για να κάνετε μια αρχική αξιολόγηση του μεγέθους του συνόλου αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="e7418-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="e7418-106">Χρησιμοποιήστε πρώτα τα φίλτρα χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e7418-106">Use time filters first.</span></span> <span data-ttu-id="e7418-107">Ιδανικά, περιορίστε τα ερωτήματά σας σε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="e7418-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="e7418-108">Στην αρχή ενός ερωτήματος, αμέσως μετά το χρονικό φίλτρο, προσθέστε τα φίλτρα που αναμένεται να καταργήσουν τα περισσότερα από τα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="e7418-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="e7418-109">Όταν αναζητάτε πλήρη διακριτικά, χρησιμοποιήστε τον τελεστή αντί για `has` `contains` το .</span><span class="sxs-lookup"><span data-stu-id="e7418-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="e7418-110">Εκτελέστε μια αναζήτηση σε μια συγκεκριμένη στήλη και όχι σε όλες τις στήλες.</span><span class="sxs-lookup"><span data-stu-id="e7418-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="e7418-111">Όταν ενώνετε πίνακες, καθορίστε πρώτα τον πίνακα με λιγότερες γραμμές.</span><span class="sxs-lookup"><span data-stu-id="e7418-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="e7418-112">`project` μόνο τις απαραίτητες στήλες από τους πίνακες που έχετε ενωθεί.</span><span class="sxs-lookup"><span data-stu-id="e7418-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="e7418-113">Για να μάθετε περισσότερα, ανατρέξτε στις [βέλτιστες πρακτικές ερωτημάτων για προχωρημένους.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="e7418-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
