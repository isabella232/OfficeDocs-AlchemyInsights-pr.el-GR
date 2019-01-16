---
title: Αντιμετώπιση προβλημάτων με σφάλματα ελέγχου ταυτότητας ροής
ms.author: kaarins
author: kaarins
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: fbb2ea4f0c6e582dae71371d958667162a138346
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291060"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="58198-102">Αντιμετώπιση προβλημάτων με σφάλματα ελέγχου ταυτότητας ροής</span><span class="sxs-lookup"><span data-stu-id="58198-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="58198-p101">Σε πολλές περιπτώσεις, οι ροές αποτύχει εξαιτίας ενός σφάλματος ελέγχου ταυτότητας. Εάν έχετε αυτόν τον τύπο του σφάλματος, το μήνυμα λάθους περιέχει "Εξουσιοδότηση" ή εμφανίζεται ο κωδικός σφάλματος 401 ή 403. Συνήθως, μπορείτε να διορθώσετε ένα σφάλμα ελέγχου ταυτότητας κατά την ενημέρωση της σύνδεσης:</span><span class="sxs-lookup"><span data-stu-id="58198-p101">In many cases, flows fail because of an authentication error. If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears. You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="58198-106">Στην κορυφή της πύλης web, κάντε κλικ στο κουμπί ή κτυπήστε το εικονίδιο του πηδαλίου για να ανοίξετε το μενού "Ρυθμίσεις", και στη συνέχεια κάντε κλικ στο κουμπί ή κτυπήστε **συνδέσεις**.</span><span class="sxs-lookup"><span data-stu-id="58198-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="58198-107">Μετακινηθείτε στη σύνδεση που είδατε στο μήνυμα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="58198-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="58198-108">Δίπλα από τη σύνδεση, κάντε κλικ στο κουμπί ή κτυπήστε την **Επιβεβαίωση κωδικού πρόσβασης** σύνδεσης στο μήνυμα σχετικά με τη σύνδεση δεν γίνεται έλεγχος ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="58198-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="58198-109">Επαλήθευση των πιστοποιήσεών σας, ακολουθώντας τις οδηγίες που εμφανίζονται, επιστρέψτε την αποτυχία εκτέλεσης ροής, και στη συνέχεια κάντε κλικ στο κουμπί ή κτυπήστε **υποβάλετε ξανά**.</span><span class="sxs-lookup"><span data-stu-id="58198-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="58198-110">Για περισσότερη βοήθεια, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων σε μια ροή](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="58198-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

