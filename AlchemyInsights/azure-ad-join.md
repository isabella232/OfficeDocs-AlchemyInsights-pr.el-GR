---
title: Συμμετοχή στο Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405060"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="4c6e0-102">Συμμετοχή στο Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4c6e0-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="4c6e0-103">Εάν ρυθμίζετε καταχωρήσεις συσκευών για πρώτη φορά, βεβαιωθείτε ότι έχετε ελέγξει την Εισαγωγή στη διαχείριση συσκευών στο [Azure Active Directory,](/azure/active-directory/devices/overview) η οποία θα σας καθοδηγήσει σχετικά με τον τρόπο με τον οποίο μπορείτε να ρυθμίσετε τις συσκευές στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c6e0-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="4c6e0-104">Εάν καταχωρείτε συσκευές απευθείας στο Azure AD και τις εγγράφετε στο Intune, θα πρέπει πρώτα [](/mem/intune/fundamentals/licenses-assign) να βεβαιωθείτε ότι έχετε ρυθμίσει τις παραμέτρους του [Intune](/mem/intune/enrollment/device-enrollment) και ότι έχετε ήδη ρυθμίσει τις άδειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="4c6e0-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="4c6e0-105">Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να εκτελείτε λειτουργίες στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c6e0-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="4c6e0-106">Μόνο ένας καθολικός διαχειριστής στο Azure AD μπορεί να διαχειριστεί τις ρυθμίσεις για τις καταχωρήσεις συσκευών.</span><span class="sxs-lookup"><span data-stu-id="4c6e0-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="4c6e0-107">Για να κάνετε την υλοποίηση συμμετοχής στο Azure AD, [ανατρέξτε στο θέμα Σχεδιασμός συμμετοχής στο Azure AD.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="4c6e0-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="4c6e0-108">Για περισσότερες λεπτομέρειες σχετικά με την επίλυση συνηθισμένων προβλημάτων με τη συμμετοχή στο Azure AD, ανατρέξτε στο θέμα Συνήθεις ερωτήσεις συμμετοχής στο [Azure Ad Join](/azure/active-directory/devices/faq) και για συσκευή Windows 10 Pro, ανατρέξτε στο θέμα Δεν είναι δυνατή η συμμετοχή του υπολογιστή Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)στο Azure AD - Πρέπει να κάνετε αναβάθμιση σε - Κοινότητα της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4c6e0-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
