---
title: Αντιμετώπιση προβλήματος-ο χρήστης δεν βρέθηκε στον κατάλογο
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768801"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="50839-102">Αντιμετώπιση προβλήματος-ο χρήστης δεν βρέθηκε στον κατάλογο</span><span class="sxs-lookup"><span data-stu-id="50839-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="50839-103">Εάν οι χρήστες λαμβάνουν μήνυμα λάθους "ο χρήστης δεν μπορεί να βρεθεί" στον κατάλογο, δοκιμάστε ξανά όπου ο τύπος θέματος είναι χρήστης δεν στον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="50839-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="50839-104">Μπορείτε να ολοκληρώσετε τα παρακάτω βήματα για να αντιμετωπίσετε το ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="50839-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="50839-105">Βεβαιωθείτε ότι ο λογαριασμός που αποδέχθηκε την πρόσκληση ηλεκτρονικού ταχυδρομείου είναι ο ίδιος λογαριασμός που χρησιμοποιείται για να εισέλθετε αργότερα.</span><span class="sxs-lookup"><span data-stu-id="50839-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="50839-106">Βεβαιωθείτε ότι ο χρήστης χρησιμοποιεί τον ίδιο λογαριασμό για να αποδεχθεί την πρόσκληση και να εισέλθετε στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="50839-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="50839-107">Για περισσότερες πληροφορίες, ανατρέξτε στο άρθρο [Τρόπος διαχείρισης ψευδωνύμων για το</a> λογαριασμό Microsoft για τη διαχείριση της σύνδεσης του Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="50839-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="50839-108">Περιηγηθείτε σε κάθε τοποθεσία (ες) στην οποία ο χρήστης λαμβάνει το σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="50839-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="50839-109">Προσθέστε την επιλογή "/_layouts/15/OLL.asx/metessfl = 0" (μέσα στα διπλά εισαγωγικά) στο τέλος της διεύθυνσης URL της τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="50839-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="50839-110">Παράδειγμα: https://< "Ηλιοτεχνική >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="50839-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="50839-111">Επιλέξτε το χρήστη από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="50839-111">Select the user from the list.</span></span>

- <span data-ttu-id="50839-112">Κάντε κλικ στην επιλογή **Κατάργηση δικαιωμάτων χρήστη** από την κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="50839-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="50839-113">Προσθέστε πίσω το χρήστη και στείλτε ξανά την πρόσκληση στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="50839-113">Add back the User and Resend the invite to the user.</span></span>

