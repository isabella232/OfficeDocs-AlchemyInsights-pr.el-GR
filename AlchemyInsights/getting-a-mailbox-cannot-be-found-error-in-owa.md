---
title: 126 Δεν είναι δυνατή η λήψη γραμματοκιβωτίου στο OWA;
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426662"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="8d9da-102">Δεν βρέθηκε κάποιο μήνυμα σφάλματος γραμματοκιβωτίου στο Outlook στο web;</span><span class="sxs-lookup"><span data-stu-id="8d9da-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="8d9da-103">Εάν χρησιμοποιείτε το Outlook στο web και  δεν μπορείτε να βρείτε ένα γραμματοκιβώτιο για σφάλμα, ο λογαριασμός που χρησιμοποιήσατε για να συνδεθείτε στο Outlook στο web δεν έχει άδεια χρήσης του Exchange Online και, επομένως, κανένα γραμματοκιβώτιο δεν συσχετίζεται με το λογαριασμό.</span><span class="sxs-lookup"><span data-stu-id="8d9da-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="8d9da-104">Ο διαχειριστής σας μπορεί να εκχωρήσει μια άδεια χρήσης στο λογαριασμό σας, ακολουθώντας τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="8d9da-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="8d9da-105">Ανοίξτε το Κέντρο διαχείρισης του Microsoft  [365](https://portal.office.com/adminportal/home#/homepage) και μεταβείτε στην ενότητα "Ενεργοί χρήστες" στην ενότητα "Χρήστες" και επιλέξτε το χρήστη που βλέπει το σφάλμα. </span><span class="sxs-lookup"><span data-stu-id="8d9da-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="8d9da-106">Στη σελίδα χρήστη που ανοίγει,  μεταβείτε στην ενότητα "Άδειες χρήσης και εφαρμογές", επιλέξτε την κατάλληλη τιμή **τοποθεσίας** και εκχωρήστε μια άδεια χρήσης που περιέχει το Exchange Online (αναπτύξτε την άδεια χρήσης για να δείτε τις λεπτομέρειες).</span><span class="sxs-lookup"><span data-stu-id="8d9da-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="8d9da-107">Όταν τελειώσετε, κάντε κλικ στην επιλογή **"Αποθήκευση αλλαγών".**</span><span class="sxs-lookup"><span data-stu-id="8d9da-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="8d9da-108">Σε ορισμένες περιπτώσεις, εάν η άδεια χρήσης έχει ήδη εκχωρηθεί σε ένα λογαριασμό χρήστη, η κατάργηση και η εκ νέου εκχώρηση της άδειας χρήσης σάς βοηθά να επιλύσετε το πρόβλημα και να την εκχωρήσετε σωστά στο σύστημα:</span><span class="sxs-lookup"><span data-stu-id="8d9da-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="8d9da-109">Ελέγξτε εάν οι συνδρομές του M365 Exchange Online (και άλλες, εάν έχετε) είναι τρέχουσες και δεν έχουν λήξει πρόσφατα.</span><span class="sxs-lookup"><span data-stu-id="8d9da-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="8d9da-110">Αφού βεβαιωθείτε ότι η συνδρομή σας δεν έχει λήξει και έχει εκχωρηθεί μια έγκυρη άδεια χρήσης στο λογαριασμό χρήστη, μπορεί να χρειαστεί έως και 24 ώρες για να γίνει προμήθεια της άδειας χρήσης, επομένως ίσως χρειαστεί να περιμένετε να επιλυθεί το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="8d9da-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="8d9da-111">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Εκχώρηση και διαχείριση αδειών χρήσης.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="8d9da-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>