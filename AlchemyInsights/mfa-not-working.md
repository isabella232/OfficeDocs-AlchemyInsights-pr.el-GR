---
title: Προβλήματα με το ΣΠΙ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755131"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="531bd-102">Προβλήματα με το Azure ΣΠΙ</span><span class="sxs-lookup"><span data-stu-id="531bd-102">Issues with Azure MFA</span></span>
<span data-ttu-id="531bd-103">Υπάρχουν μερικά πράγματα που πρέπει να εξετάσετε εάν οι χρήστες δεν μπορούν να συνδεθούν χρησιμοποιώντας τον έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)</span><span class="sxs-lookup"><span data-stu-id="531bd-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="531bd-104">Ο χρήστης που επηρεάζεται μπορεί να αποκλειστεί στην πύλη του Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="531bd-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="531bd-105">Σε αυτή την περίπτωση, οι προσπάθειες ελέγχου ταυτότητας για τον συγκεκριμένο χρήστη θα απορριφθούν αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="531bd-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="531bd-106">Ακολουθήστε τα βήματα που περιέχετε σε αυτό το άρθρο για να καταργήσετε τον αποκλεισμό τους.</span><span class="sxs-lookup"><span data-stu-id="531bd-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="531bd-107">Εάν ο αποκλεισμός του χρήστη δεν βοήθησε ή ο χρήστης δεν αποκλειστεί, μπορείτε να δοκιμάσετε να επαναφέρετε το ΣΠΙ για το χρήστη και θα περάσουν από τη διαδικασία εγγραφής ξανά.</span><span class="sxs-lookup"><span data-stu-id="531bd-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="531bd-108">Ακολουθήστε τα βήματα που περιλάβετε σε αυτό το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="531bd-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="531bd-109">Εάν αυτή είναι η πρώτη φορά που ενεργοποιήσατε το ΣΠΙ και οι χρήστες σας δεν μπορούν να συνδεθούν σε προγράμματα-πελάτες που δεν χρησιμοποιούν προγράμματα περιήγησης, όπως το Outlook, το Skype, το κ. λπ., ίσως το ADAL (βιβλιοθήκη ελέγχου ταυτότητας της υπηρεσίας καταλόγου Active Directory) δεν είναι ενεργοποιημένο στη συνδρομή σας στο O365.</span><span class="sxs-lookup"><span data-stu-id="531bd-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="531bd-110">Σε αυτή την περίπτωση, θα πρέπει να συνδεθείτε στο Exchange Online PowerShell και να εκτελέσετε αυτό το cmdlet:  *OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="531bd-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>