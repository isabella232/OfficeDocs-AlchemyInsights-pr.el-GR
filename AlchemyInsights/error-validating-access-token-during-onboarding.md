---
title: Παρουσιάστηκε σφάλμα κατά την επικύρωση του σφάλματος διακριτικού πρόσβασης κατά την επιβίβαση στην ανάλυση επιφάνειας εργασίας
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741184"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="adf56-102">Εμφανίζεται το μήνυμα λάθους "Παρουσιάστηκε σφάλμα επικύρωσης διακριτικού πρόσβασης" κατά τη διάρκεια της ανάλυσης επιφάνειας εργασίας</span><span class="sxs-lookup"><span data-stu-id="adf56-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="adf56-103">Αυτό το σφάλμα παρατηρείται συνήθως όταν λήξει το διακριτικό ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="adf56-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="adf56-104">Συνήθως, η ανανέωση της σελίδας ανανεώνει το διακριτικό.</span><span class="sxs-lookup"><span data-stu-id="adf56-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="adf56-105">Ωστόσο, αυτό το ζήτημα μπορεί να επιμείνει εάν υπάρχουν πολιτικές υπό όρους πρόσβασης που εφαρμόζονται στο λογαριασμό που χρησιμοποιείται για την ανάλυση επιφάνειας εργασίας επί του σκάφους.</span><span class="sxs-lookup"><span data-stu-id="adf56-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="adf56-106">Μπορείτε να αναθεωρήσετε τα αρχεία καταγραφής σύνδεσης Azure AD στην πύλη Azure για να δείτε αν υπάρχουν τυχόν αποτυχίες εισόδου για το λογαριασμό που χρησιμοποιείται για την καταγραφή της ανάλυσης επιφάνειας εργασίας.</span><span class="sxs-lookup"><span data-stu-id="adf56-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="adf56-107">Για περισσότερες πληροφορίες σχετικά με την υπό όρους πρόσβαση, επισκεφθείτε [το πρόγραμμα ανάπτυξης υπό όρους πρόσβασης](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="adf56-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>