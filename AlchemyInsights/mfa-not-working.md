---
title: Προβλήματα με το MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810484"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="84049-102">Προβλήματα με το Azure MFA</span><span class="sxs-lookup"><span data-stu-id="84049-102">Issues with Azure MFA</span></span>
<span data-ttu-id="84049-103">Υπάρχουν μερικά πράγματα που πρέπει να ελέγξετε εάν οι χρήστες δεν μπορούν να συνδεθούν χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων (MFA)</span><span class="sxs-lookup"><span data-stu-id="84049-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="84049-104">Ο χρήστης που επηρεάζεται ενδέχεται να αποκλειστεί στην πύλη azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="84049-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="84049-105">Σε αυτή την περίπτωση, οι προσπάθειες ελέγχου ταυτότητας για τον συγκεκριμένο χρήστη θα αποτεφράονται αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="84049-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="84049-106">Ακολουθήστε τα βήματα σε αυτό το άρθρο για να τα ξεμπλοκάρει.</span><span class="sxs-lookup"><span data-stu-id="84049-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="84049-107">Εάν η κατάργηση του αποκλεισμού του χρήστη δεν βοήθησε ή ο χρήστης δεν αποκλειστεί, μπορείτε να προσπαθήσετε να επαναφέρετε το MFA για το χρήστη και θα περάσει ξανά τη διαδικασία εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="84049-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="84049-108">Ακολουθήστε τα βήματα σε αυτό το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="84049-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="84049-109">Εάν αυτή είναι η πρώτη φορά που έχετε ενεργοποιήσει το MFA και οι χρήστες σας δεν μπορούν να συνδεθείτε σε προγράμματα-πελάτες που δεν είναι προγράμματα περιήγησης, όπως το Outlook, το Skype κ.λπ., ίσως το ADAL (Βιβλιοθήκη ελέγχου ταυτότητας Active Directory) να μην είναι ενεργοποιημένο στη συνδρομή σας στο O365.</span><span class="sxs-lookup"><span data-stu-id="84049-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="84049-110">Σε αυτή την περίπτωση, θα πρέπει να συνδεθείτε στο Exchange Online Powershell και να εκτελέσετε αυτό το cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="84049-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>