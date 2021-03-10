---
title: Εφαρμογή βέλτιστων πρακτικών για σύνθετα ερωτήματα αναζήτησης
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694274"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="57e1f-102">Εφαρμογή βέλτιστων πρακτικών για σύνθετα ερωτήματα αναζήτησης</span><span class="sxs-lookup"><span data-stu-id="57e1f-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="57e1f-103">Για να λάβετε αποτελέσματα πιο γρήγορα και για να αποφύγετε χρονικά αποτελέσματα κατά την εκτέλεση σύνθετων ερωτημάτων, εφαρμόστε αυτές τις βέλτιστες πρακτικές:</span><span class="sxs-lookup"><span data-stu-id="57e1f-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="57e1f-104">Όταν προσπαθείτε να δημιουργήσετε νέα ερωτήματα, χρησιμοποιείτε πάντα ένα όριο, για να αποφύγετε τη λήψη εξαιρετικά μεγάλων συνόλων αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="57e1f-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="57e1f-105">Επίσης, χρησιμοποιήστε `count` το για να κάνετε μια αρχική αξιολόγηση του μεγέθους του συνόλου αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="57e1f-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="57e1f-106">Χρησιμοποιήστε πρώτα τα φίλτρα χρόνου.</span><span class="sxs-lookup"><span data-stu-id="57e1f-106">Use time filters first.</span></span> <span data-ttu-id="57e1f-107">Ιδανικά, περιορίστε τα ερωτήματά σας σε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="57e1f-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="57e1f-108">Στην αρχή ενός ερωτήματος, αμέσως μετά το χρονικό φίλτρο, προσθέστε τα φίλτρα που αναμένεται να καταργήσουν τα περισσότερα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="57e1f-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="57e1f-109">Όταν αναζητάτε πλήρη διακριτικά, χρησιμοποιήστε τον τελεστή αντί για το `has` `contains` .</span><span class="sxs-lookup"><span data-stu-id="57e1f-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="57e1f-110">Εκτελέστε μια αναζήτηση σε μια συγκεκριμένη στήλη και όχι σε όλες τις στήλες.</span><span class="sxs-lookup"><span data-stu-id="57e1f-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="57e1f-111">Κατά τη σύνδεση πινάκων, καθορίστε πρώτα τον πίνακα με λιγότερες γραμμές.</span><span class="sxs-lookup"><span data-stu-id="57e1f-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="57e1f-112">`project` μόνο τις απαραίτητες στήλες από τους πίνακες που έχετε ενωθεί.</span><span class="sxs-lookup"><span data-stu-id="57e1f-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="57e1f-113">Για να μάθετε περισσότερα, ανατρέξτε στις [βέλτιστες πρακτικές ερωτήματος για προχωρημένους.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="57e1f-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
