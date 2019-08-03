---
title: Αντιμετώπιση προβλημάτων σχετικά με το ζήτημα - ο χρήστης δεν βρέθηκε στον κατάλογο
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249913"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="41679-102">Αντιμετώπιση προβλημάτων σχετικά με το ζήτημα - ο χρήστης δεν βρέθηκε στον κατάλογο</span><span class="sxs-lookup"><span data-stu-id="41679-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="41679-103">Εάν οι χρήστες λαμβάνουν το σφάλμα μήνυμα "δεν είναι δυνατή η εύρεση χρήστη" στον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="41679-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="41679-104">Προσπαθήστε ξανά όταν ο τύπος θέματος χρήστη δεν βρίσκεται στον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="41679-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="41679-105">Τα ακόλουθα βήματα μπορεί να ολοκληρωθεί για να αντιμετωπίσετε το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="41679-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="41679-106">Βεβαιωθείτε ότι ο λογαριασμός που έγινε αποδεκτή την πρόσκληση e-mail είναι ο ίδιος λογαριασμός που χρησιμοποιείται για να εισέλθετε αργότερα.</span><span class="sxs-lookup"><span data-stu-id="41679-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="41679-107">Βεβαιωθείτε ότι ο χρήστης χρησιμοποιεί τον ίδιο λογαριασμό για να αποδεχτείτε την πρόσκληση και να εισέλθετε στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="41679-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="41679-108">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Πώς να διαχειρίζεστε τα ψευδώνυμα για το λογαριασμό σας Microsoft</a> για τη διαχείριση της σύνδεσης του Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="41679-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="41679-109">Αναζητήστε κάθε τοποθεσιών στις οποίες ο χρήστης λαμβάνει το σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="41679-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="41679-110">Προσθέστε "/ _layouts/15/people.aspx/membershipgroupid=0" (μέσα σε διπλά εισαγωγικά) στο τέλος της διεύθυνσης URL της τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="41679-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="41679-111">Παράδειγμα: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="41679-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="41679-112">Επιλέξτε το χρήστη από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="41679-112">Select the user from the list.</span></span>

- <span data-ttu-id="41679-113">Κάντε κλικ στο κουμπί **Κατάργηση δικαιωμάτων χρήστη** από την κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="41679-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="41679-114">Προσθέστε ξανά το χρήστη και στείλτε ξανά την πρόσκληση στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="41679-114">Add back the User and Resend the invite to the user.</span></span>

