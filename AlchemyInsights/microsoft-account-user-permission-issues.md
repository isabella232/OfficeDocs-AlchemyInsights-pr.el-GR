---
title: Αντιμετώπιση προβλημάτων ζητήματος-ο χρήστης δεν βρέθηκε στον κατάλογο
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725407"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="43c8c-102">Αντιμετώπιση προβλημάτων ζητήματος-ο χρήστης δεν βρέθηκε στον κατάλογο</span><span class="sxs-lookup"><span data-stu-id="43c8c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="43c8c-103">Εάν οι χρήστες λαμβάνουν μήνυμα σφάλματος "δεν είναι δυνατή η εύρεση του χρήστη" στον κατάλογο, δοκιμάστε ξανά όπου ο τύπος θέματος είναι χρήστης που δεν βρίσκεται στον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="43c8c-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="43c8c-104">Μπορείτε να ολοκληρώσετε τα παρακάτω βήματα για να αντιμετωπίσετε το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="43c8c-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="43c8c-105">Βεβαιωθείτε ότι ο λογαριασμός που αποδέχτηκε την πρόσκληση ηλεκτρονικού ταχυδρομείου είναι ο ίδιος λογαριασμός που χρησιμοποιείται για την είσοδό σας αργότερα.</span><span class="sxs-lookup"><span data-stu-id="43c8c-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="43c8c-106">Βεβαιωθείτε ότι ο χρήστης χρησιμοποιεί τον ίδιο λογαριασμό για να αποδεχθεί την πρόσκληση και να πραγματοποιήσει είσοδο στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="43c8c-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="43c8c-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Πώς μπορείτε να διαχειριστείτε ψευδώνυμα για το λογαριασμό σας Microsoft </a> για να διαχειριστείτε τη σύνδεση Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="43c8c-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="43c8c-108">Μεταβείτε σε κάθε τοποθεσία (ες) όπου ο χρήστης λαμβάνει το σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="43c8c-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="43c8c-109">Προσθήκη "/_layouts/15/People.aspx/membershipgroupid = 0" (εντός των διπλών εισαγωγικών) στο άκρο της διεύθυνσης URL της τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="43c8c-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="43c8c-110">Παράδειγμα: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="43c8c-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="43c8c-111">Επιλέξτε το χρήστη από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="43c8c-111">Select the user from the list.</span></span>

- <span data-ttu-id="43c8c-112">Κάντε κλικ στην επιλογή **Κατάργηση δικαιωμάτων χρήστη** από την κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="43c8c-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="43c8c-113">Προσθέστε ξανά το χρήστη και στείλτε ξανά την πρόσκληση στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="43c8c-113">Add back the User and Resend the invite to the user.</span></span>

