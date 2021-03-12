---
title: Αντιμετώπιση προβλημάτων απρόσκοπτης σύνδεσης (SSO) που βασίζονται σε κωδικό πρόσβασης
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714768"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="1d365-102">Αντιμετώπιση προβλημάτων απρόσκοπτης σύνδεσης (SSO) που βασίζονται σε κωδικό πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="1d365-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="1d365-103">Για να μάθετε τα βασικά στοιχεία της SSO που βασίζεται σε κωδικό πρόσβασης, ανατρέξτε στο θέμα ["Έλεγχος ταυτότητας βάσει κωδικού πρόσβασης" με το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="1d365-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="1d365-104">**Ρύθμιση παραμέτρων SSO βάσει κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="1d365-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="1d365-105">[Ρύθμιση παραμέτρων της μεμονωμένης σύνδεσης που βασίζεται σε](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) κωδικό πρόσβασης - Αυτό το άρθρο περιγράφει πιο αναλυτικά την επιλογή SSO που βασίζεται σε κωδικό πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="1d365-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="1d365-106">Εάν η εφαρμογή που προσθέτετε απαιτεί προσαρμοσμένη ρύθμιση παραμέτρων και πρέπει να χρησιμοποιήσετε SSO που βασίζεται σε κωδικό πρόσβασης, αυτό το άρθρο είναι για εσάς.</span><span class="sxs-lookup"><span data-stu-id="1d365-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="1d365-107">[Ρυθμίστε τις παραμέτρους μίας σύνδεσης που βασίζεται σε](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) κωδικό πρόσβασης για εφαρμογές εσωτερικής αποθήκευσης - Ο διακομιστής μεσολάβησης εφαρμογών υποστηρίζει πολλές λειτουργίες μονής σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="1d365-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="1d365-108">Η σύνδεση που βασίζεται σε κωδικό πρόσβασης προορίζεται για εφαρμογές που χρησιμοποιούν συνδυασμό ονόματος χρήστη/κωδικού πρόσβασης για τον έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="1d365-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="1d365-109">Όταν ρυθμίζετε τις παραμέτρους της σύνδεσης με κωδικό πρόσβασης για την εφαρμογή σας, οι χρήστες πρέπει να πραγματοποιήσουν είσοδο στην εφαρμογή εσωτερικής εγκατάστασης μία φορά.</span><span class="sxs-lookup"><span data-stu-id="1d365-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="1d365-110">Μετά από αυτό, το Azure Active Directory αποθηκεύει τις πληροφορίες σύνδεσης και τις παρέχει αυτόματα στην εφαρμογή, όταν οι χρήστες σας έχουν πρόσβαση σε αυτές από απόσταση.</span><span class="sxs-lookup"><span data-stu-id="1d365-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="1d365-111">Θα πρέπει να έχετε ήδη δημοσιεύσει και δοκιμάσει την εφαρμογή σας με διακομιστή μεσολάβησης εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="1d365-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="1d365-112">Εάν όχι, ακολουθήστε τα βήματα στη δημοσίευση εφαρμογών χρησιμοποιώντας το διακομιστή μεσολάβησης εφαρμογών [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) στη συνέχεια, συνεχίστε με τη ρύθμιση παραμέτρων SSO που βασίζεται σε κωδικό πρόσβασης για εφαρμογές on-prem.</span><span class="sxs-lookup"><span data-stu-id="1d365-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="1d365-113">Για την αντιμετώπιση προβλημάτων SSO που βασίζεται σε κωδικό πρόσβασης, ανατρέξτε στο θέμα "Αντιμετώπιση προβλημάτων μονής σύνδεσης βάσει κωδικού [πρόσβασης στο Azure AD"](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="1d365-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
