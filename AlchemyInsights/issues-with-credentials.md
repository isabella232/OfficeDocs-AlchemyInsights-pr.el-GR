---
title: Προβλήματα με διαπιστευτήρια
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063629"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="ece9b-102">Προβλήματα με διαπιστευτήρια</span><span class="sxs-lookup"><span data-stu-id="ece9b-102">Issues with credentials</span></span>

<span data-ttu-id="ece9b-103">Η πλατφόρμα ταυτότητας της Microsoft και η ροή διαπιστευτηρίων προγράμματος-πελάτη [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) περιγράφουν πώς μπορείτε να προγραμματίσετε απευθείας σε σχέση με τα διαπιστευτήρια προγράμματος-πελάτη OAuth 2.0 που εκ παρέχουν ροή.</span><span class="sxs-lookup"><span data-stu-id="ece9b-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="ece9b-104">**Πώς μπορώ να διαχειριστώ τον κωδικό πρόσβασης ή τα διαπιστευτήρια πιστοποιητικού μιας εφαρμογής;**</span><span class="sxs-lookup"><span data-stu-id="ece9b-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="ece9b-105">Στο Azure CLI, μπορείτε να χρησιμοποιήσετε τα διαπιστευτήρια της εφαρμογής [az ad για](https://docs.microsoft.com/cli/azure/ad/app/credential) τη διαγραφή, τη λίστα ή την επαναφορά των διαπιστευτηρίων κωδικού πρόσβασης ή πιστοποιητικού μιας εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="ece9b-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="ece9b-106">**Πώς μπορούν οι χρήστες μου να επαναφέρουν τους κωδικούς πρόσβασής τους;**</span><span class="sxs-lookup"><span data-stu-id="ece9b-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="ece9b-107">Οι χρήστες πρέπει να [εγγραφούν για επαναφορά κωδικού πρόσβασης από το χρήστη για](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) να μπορούν να επαναφέρουν τους κωδικούς πρόσβασής τους.</span><span class="sxs-lookup"><span data-stu-id="ece9b-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="ece9b-108">Μόλις ένας χρήστης εγγραφεί, μπορεί να ακολουθήσει τις οδηγίες σε αυτό το άρθρο για να επαναφέρετε τον κωδικό πρόσβασής του: [Επαναφέρετε τον κωδικό πρόσβασης της εργασίας ή του σχολείου σας.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="ece9b-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="ece9b-109">**Πώς μπορούν οι χρήστες μου να αλλάξουν τους κωδικούς πρόσβασής τους;**</span><span class="sxs-lookup"><span data-stu-id="ece9b-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="ece9b-110">Οι χρήστες μπορούν να ακολουθήσουν τα βήματα που αναφέρονται σε αυτό το άρθρο για να αλλάξουν τους κωδικούς πρόσβασής τους: [Πώς να αλλάξουν τον κωδικό πρόσβασής σας.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="ece9b-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="ece9b-111">Μπορούν επίσης να [διαχειρίζονται κωδικούς πρόσβασης εφαρμογών για επαλήθευση σε δύο βήματα.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="ece9b-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="ece9b-112">**Εμφανίζεται ένα σφάλμα στο χρήστη μου κατά την αλλαγή ή την επαναφορά του κωδικού πρόσβασής του**</span><span class="sxs-lookup"><span data-stu-id="ece9b-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="ece9b-113">Αυτή η σύνδεση θα παρέχει πληροφορίες σχετικά με συνήθη προβλήματα που μπορεί να προκύψουν όταν ένας χρήστης προσπαθεί να επαναφέρει τον κωδικό πρόσβασής του: [Συνήθη προβλήματα και λύσεις](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="ece9b-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="ece9b-114">**Δεν μπορώ να επαναφέρετε τον κωδικό πρόσβασης ενός χρήστη**</span><span class="sxs-lookup"><span data-stu-id="ece9b-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="ece9b-115">Βεβαιωθείτε ότι έχετε την άδεια να επαναφέρετε τους κωδικούς πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="ece9b-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="ece9b-116">*Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές κωδικών πρόσβασης και οι διαχειριστές χρηστών μπορούν να επαναφέρουν τους κωδικούς πρόσβασης των χρηστών.*</span><span class="sxs-lookup"><span data-stu-id="ece9b-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ece9b-117">Οι καθολικοί διαχειριστές μπορούν επίσης να επαναφέρουν τους κωδικούς πρόσβασης άλλου διαχειριστή με δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="ece9b-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="ece9b-118">Βεβαιωθείτε ότι έχετε κατανοήσει τις απαιτήσεις άδειας χρήσης:</span><span class="sxs-lookup"><span data-stu-id="ece9b-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="ece9b-119">Πρέπει να έχετε εκχωρήσει τουλάχιστον μία άδεια χρήσης στον οργανισμό σας:</span><span class="sxs-lookup"><span data-stu-id="ece9b-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="ece9b-120">**Χρήστες μόνο για cloud** - Οποιαδήποτε SKU επί πληρωμή για το Office 365 (O365) ή Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="ece9b-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="ece9b-121">**Χρήστες cloud ή/και** εσωτερικής εγκατάστασης - Azure AD Premium P1 ή P2, Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια (EMS) ή Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="ece9b-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="ece9b-122">Για να μάθετε περισσότερα σχετικά με τις απαιτήσεις άδειας χρήσης, [ανατρέξτε στο θέμα "Απαιτήσεις παραχώρησης αδειών χρήσης για επαναφορά κωδικού](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)πρόσβασης του Azure AD από το χρήστη".</span><span class="sxs-lookup"><span data-stu-id="ece9b-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="ece9b-123">Για να επαναφέρετε τον κωδικό πρόσβασης ενός χρήστη, βρείτε το χρήστη στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ece9b-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="ece9b-124">Στη συνέχεια, στο πλαίσιο επισκόπησης για το χρήστη, κάντε κλικ στο κουμπί "επαναφορά κωδικού πρόσβασης".</span><span class="sxs-lookup"><span data-stu-id="ece9b-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="ece9b-125">**Το κουμπί επαναφοράς κωδικού πρόσβασης είναι γκριζαρισμένο**</span><span class="sxs-lookup"><span data-stu-id="ece9b-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="ece9b-126">Δεν έχετε εξουσιοδότηση να επαναφέρετε **τους κωδικούς** πρόσβασης αυτού του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="ece9b-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="ece9b-127">*Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές κωδικών πρόσβασης και οι διαχειριστές χρηστών μπορούν να επαναφέρουν τους κωδικούς πρόσβασης των χρηστών.*</span><span class="sxs-lookup"><span data-stu-id="ece9b-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ece9b-128">Οι καθολικοί διαχειριστές μπορούν επίσης να επαναφέρουν τους κωδικούς πρόσβασης άλλου διαχειριστή με δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="ece9b-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ece9b-129">**Δεν βλέπω το blade επαναφοράς κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="ece9b-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="ece9b-130">Δεν έχετε εξουσιοδότηση για την επαναφορά κωδικών πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="ece9b-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="ece9b-131">*Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές κωδικών πρόσβασης και οι διαχειριστές χρηστών μπορούν να επαναφέρουν τους κωδικούς πρόσβασης των χρηστών.*</span><span class="sxs-lookup"><span data-stu-id="ece9b-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ece9b-132">Οι καθολικοί διαχειριστές μπορούν επίσης να επαναφέρουν τους κωδικούς πρόσβασης άλλου διαχειριστή με δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="ece9b-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ece9b-133">**Δεν βλέπω το blade ενοποίησης εσωτερικής εγκατάστασης κατά την επαναφορά κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="ece9b-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="ece9b-134">Τα συστήματα blade ενοποίησης εσωτερικής εγκατάστασης εμφανίζονται μόνο σε υβριδικά περιβάλλοντα, που σημαίνει ότι χρησιμοποιείτε την writeback κωδικού πρόσβασης για να χειριστείτε τους κωδικούς πρόσβασης των χρηστών εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="ece9b-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="ece9b-135">Δεν βλέπετε αυτό το blade εάν:</span><span class="sxs-lookup"><span data-stu-id="ece9b-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="ece9b-136">Δεν χρησιμοποιείτε την writeback κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="ece9b-136">You are not using password writeback</span></span>
  - <span data-ttu-id="ece9b-137">Υπάρχει πρόβλημα με την εγκατάσταση/συνδεσιμότητα της writeback κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="ece9b-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="ece9b-138">Υπάρχει πρόβλημα με την εγκατάσταση/συνδεσιμότητα του Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="ece9b-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="ece9b-139">Για περισσότερα βήματα αντιμετώπισης προβλημάτων με την writeback κωδικού πρόσβασης, ανατρέξτε στην ενότητα "Αντιμετώπιση [προβλημάτων με την writeback κωδικού πρόσβασης"](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="ece9b-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="ece9b-140">**Δεν ξέρω πώς να επαναφέρω τον κωδικό πρόσβασης ενός χρήστη**</span><span class="sxs-lookup"><span data-stu-id="ece9b-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="ece9b-141">Πραγματοποιήστε είσοδο στην πύλη Azure ως κατάλληλος διαχειριστής.</span><span class="sxs-lookup"><span data-stu-id="ece9b-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="ece9b-142">Μεταβείτε στη σελίδα **"Χρήστες και ομάδες" και** επιλέξτε "Όλοι **οι χρήστες".**</span><span class="sxs-lookup"><span data-stu-id="ece9b-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="ece9b-143">Επιλέξτε ένα χρήστη από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="ece9b-143">Select a user from the list.</span></span>
4. <span data-ttu-id="ece9b-144">Για τον επιλεγμένο χρήστη, επιλέξτε **"Επισκόπηση" και,** στη συνέχεια, στη γραμμή εντολών, επιλέξτε "Επαναφορά **κωδικού πρόσβασης".**</span><span class="sxs-lookup"><span data-stu-id="ece9b-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="ece9b-145">Επιλέξτε το **κουμπί "Επαναφορά** κωδικού πρόσβασης" και ακολουθήστε τις οδηγίες στην οθόνη.</span><span class="sxs-lookup"><span data-stu-id="ece9b-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="ece9b-146">Μόνο οι επαναρυθμιώσεις που εκτελούνται μέσω της **επιστροφής κωδικού** πρόσβασης υποστήριξης της πύλης Azure.</span><span class="sxs-lookup"><span data-stu-id="ece9b-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="ece9b-147">**Έχω επαναφέρει τον κωδικό πρόσβασης ενός χρήστη εσωτερικής εγκατάστασης από την πύλη διαχείρισης του Office 365 ή την εφαρμογή του Office 365 για κινητές συσκευές, αλλά ο χρήστης εξακολουθεί να μην μπορεί να κάνει είσοδο**</span><span class="sxs-lookup"><span data-stu-id="ece9b-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="ece9b-148">Η Writeback κωδικού πρόσβασης δεν υποστηρίζεται σε αυτήν την πύλη.</span><span class="sxs-lookup"><span data-stu-id="ece9b-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="ece9b-149">Επαναφέρετε τον κωδικό πρόσβασης του χρήστη στην πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="ece9b-149">Reset the user's password again in the Azure portal.</span></span>
