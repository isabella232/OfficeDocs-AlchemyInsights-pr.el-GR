---
title: Ζητήματα μυστικών προγραμμάτων-πελατών εγγραφής εφαρμογών ή πιστοποιητικών
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404788"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="7e4a3-102">Ζητήματα μυστικών προγραμμάτων-πελατών εγγραφής εφαρμογών ή πιστοποιητικών</span><span class="sxs-lookup"><span data-stu-id="7e4a3-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="7e4a3-103">Λήξη μυστικού προγράμματος-πελάτη εφαρμογών;</span><span class="sxs-lookup"><span data-stu-id="7e4a3-103">Application client secret expiring?</span></span>

<span data-ttu-id="7e4a3-104">Ανεξάρτητα από τον τρόπο με τον οποίο δημιουργήθηκε η καταχωρημένη εφαρμογή, είτε μέσω της τυπικής διαδικασίας εγγραφής στην πύλη καταχώρησης εφαρμογών είτε εάν η Κύρια υπηρεσία δημιουργήθηκε στον μισθωτή σας χρησιμοποιώντας τη συγκατάθεση της εφαρμογής, θα πρέπει να δημιουργηθεί ένα νέο Μυστικό πελάτη πριν από τη λήξη της τρέχουσας και να ενημερωθεί στον σχετικό κωδικό εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="7e4a3-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="7e4a3-105">Η μέγιστη περίοδος ισχύος είναι 2 έτη.</span><span class="sxs-lookup"><span data-stu-id="7e4a3-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="7e4a3-106">Ως υπενθύμιση, η κρυφή τιμή πρέπει να καταγράφεται, καθώς δεν θα είναι πλέον ορατή μετά την έξοδο από τη σελίδα "Καταχωρήσεις εφαρμογών" στην πύλη.</span><span class="sxs-lookup"><span data-stu-id="7e4a3-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="7e4a3-107">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Γρήγορη εκκίνηση: Καταχωρήστε μια](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) εφαρμογή στην πλατφόρμα ταυτότητας της Microsoft και [βέλτιστες πρακτικές για την πλατφόρμα ταυτότητας της Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="7e4a3-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="7e4a3-108">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα Δημιουργία εφαρμογής Azure AD & κύρια υπηρεσία στην πύλη - Πλατφόρμα ταυτότητας της Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="7e4a3-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
