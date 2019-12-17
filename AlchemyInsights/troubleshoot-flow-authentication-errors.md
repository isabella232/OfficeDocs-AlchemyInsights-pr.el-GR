---
title: Αντιμετώπιση προβλημάτων ελέγχου ταυτότητας ροής
ms.author: pebaum
author: pebaum
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3d49d15d243dd98afc6f78b9e75f0cfa74c2cd7c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050633"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="09671-102">Αντιμετώπιση προβλημάτων ελέγχου ταυτότητας ροής</span><span class="sxs-lookup"><span data-stu-id="09671-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="09671-103">Σε πολλές περιπτώσεις, οι ροές αποτυγχάνουν εξαιτίας ενός σφάλματος ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="09671-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="09671-104">Εάν έχετε αυτόν τον τύπο σφάλματος, το μήνυμα λάθους περιέχει "μη εξουσιοδοτημένη" ή εμφανίζεται ένας κωδικός σφάλματος 401 ή 403.</span><span class="sxs-lookup"><span data-stu-id="09671-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="09671-105">Συνήθως, μπορείτε να διορθώσετε ένα σφάλμα ελέγχου ταυτότητας ενημερώνοντας τη σύνδεση:</span><span class="sxs-lookup"><span data-stu-id="09671-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="09671-106">Στο επάνω μέρος της πύλης Web, κάντε κλικ ή πατήστε το εικονίδιο με το γρανάζι για να ανοίξετε το μενού ρυθμίσεις και, στη συνέχεια, κάντε κλικ ή πατήστε **συνδέσεις**.</span><span class="sxs-lookup"><span data-stu-id="09671-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="09671-107">Μετακινηθείτε στη σύνδεση για την οποία είδατε το μήνυμα σφάλματος μη εξουσιοδοτημένο.</span><span class="sxs-lookup"><span data-stu-id="09671-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="09671-108">Δίπλα στη σύνδεση, κάντε κλικ ή πατήστε τη σύνδεση **Επιβεβαιώστε τον κωδικό πρόσβασης** στο μήνυμα σχετικά με τη σύνδεση που δεν έχει γίνει έλεγχος ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="09671-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="09671-109">Επαληθεύστε τα διαπιστευτήριά σας, ακολουθώντας τις οδηγίες που εμφανίζονται, επιστρέψτε στην αποτυχία εκτέλεσης ροής και, στη συνέχεια, κάντε κλικ ή πατήστε Επανάληψη **υποβολής.**</span><span class="sxs-lookup"><span data-stu-id="09671-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="09671-110">Για περισσότερη βοήθεια, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων ροής](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="09671-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

