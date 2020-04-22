---
title: Αντιμετώπιση προβλημάτων - Ο χρήστης δεν βρέθηκε στον κατάλογο
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702738"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6594f-102">Αντιμετώπιση προβλημάτων - Ο χρήστης δεν βρέθηκε στον κατάλογο</span><span class="sxs-lookup"><span data-stu-id="6594f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6594f-103">Εάν οι χρήστες λαμβάνουν το μήνυμα λάθους «ο χρήστης δεν μπορεί να βρεθεί» στον κατάλογο, προσπαθήστε πάλι όπου ο τύπος ζητημάτων είναι χρήστης όχι στον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="6594f-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6594f-104">Τα ακόλουθα βήματα μπορούν να ολοκληρωθούν για την αντιμετώπιση του ζητήματος.</span><span class="sxs-lookup"><span data-stu-id="6594f-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6594f-105">Βεβαιωθείτε ότι ο λογαριασμός που αποδέχθηκε την πρόσκληση ηλεκτρονικού ταχυδρομείου είναι ο ίδιος λογαριασμός που χρησιμοποιείται για είσοδο αργότερα.</span><span class="sxs-lookup"><span data-stu-id="6594f-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6594f-106">Βεβαιωθείτε ότι ο χρήστης χρησιμοποιεί τον ίδιο λογαριασμό για να αποδεχτεί την πρόσκληση και να συνδεθεί στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="6594f-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6594f-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τρόπος διαχείρισης</a> ψευδωνύμων για το λογαριασμό Microsoft για τη διαχείριση της σύνδεσης Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="6594f-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6594f-108">Μεταβείτε σε κάθε τοποθεσία ή τις οποίες ο χρήστης λαμβάνει το σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="6594f-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6594f-109">Προσθέστε "/_layouts/15/people.aspx/membershipgroupid=0" (μέσα στα διπλά εισαγωγικά) στο τέλος της διεύθυνσης URL της τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="6594f-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6594f-110">Παράδειγμα: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6594f-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6594f-111">Επιλέξτε το χρήστη από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="6594f-111">Select the user from the list.</span></span>

- <span data-ttu-id="6594f-112">Κάντε κλικ στην επιλογή **Κατάργηση δικαιωμάτων χρήστη** από την Κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="6594f-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6594f-113">Προσθέστε ξανά το χρήστη και στείλτε ξανά την πρόσκληση στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="6594f-113">Add back the User and Resend the invite to the user.</span></span>

