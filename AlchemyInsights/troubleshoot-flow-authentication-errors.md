---
title: Αντιμετώπιση σφαλμάτων ελέγχου ταυτότητας ροής
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690567"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="cc67b-102">Αντιμετώπιση σφαλμάτων ελέγχου ταυτότητας ροής</span><span class="sxs-lookup"><span data-stu-id="cc67b-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="cc67b-103">Σε πολλές περιπτώσεις, οι ροές αποτυγχάνουν εξαιτίας ενός σφάλματος ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="cc67b-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="cc67b-104">Εάν έχετε αυτόν τον τύπο σφάλματος, το μήνυμα σφάλματος περιέχει τη φράση "μη εξουσιοδοτημένη εργασία" ή εμφανίζεται ένας κωδικός σφάλματος 401 ή 403.</span><span class="sxs-lookup"><span data-stu-id="cc67b-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="cc67b-105">Συνήθως, μπορείτε να διορθώσετε ένα σφάλμα ελέγχου ταυτότητας, ενημερώνοντας τη σύνδεση:</span><span class="sxs-lookup"><span data-stu-id="cc67b-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="cc67b-106">Στο επάνω μέρος της πύλης Web, κάντε κλικ ή πατήστε το εικονίδιο γραναζιού για να ανοίξετε το μενού ρυθμίσεις και, στη συνέχεια, κάντε κλικ ή πατήστε **συνδέσεις**.</span><span class="sxs-lookup"><span data-stu-id="cc67b-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="cc67b-107">Πραγματοποιήστε κύλιση στη σύνδεση για την οποία είδατε το μη εξουσιοδοτημένο μήνυμα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="cc67b-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="cc67b-108">Δίπλα στη σύνδεση, κάντε κλικ ή πατήστε τη σύνδεση **Επαλήθευση κωδικού πρόσβασης** στο μήνυμα σχετικά με τη μη επικύρωση της σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="cc67b-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="cc67b-109">Επαληθεύστε τα διαπιστευτήριά σας ακολουθώντας τις οδηγίες που εμφανίζονται, επιστρέψτε στην αποτυχία εκτέλεσης ροής και, στη συνέχεια, κάντε κλικ ή πατήστε **ξανά**.</span><span class="sxs-lookup"><span data-stu-id="cc67b-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="cc67b-110">Για περισσότερη βοήθεια, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων ροής](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="cc67b-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

