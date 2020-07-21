---
title: Ο χρήστης λαμβάνει σφάλμα AADSTS7000112 Το Yammer είναι απενεργοποιημένο
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198060"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="72b30-102">Ο χρήστης λαμβάνει σφάλμα AADSTS7000112 Το Yammer είναι απενεργοποιημένο</span><span class="sxs-lookup"><span data-stu-id="72b30-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="72b30-103">Εάν εμφανιστεί το σφάλμα "AADSTS7000112: Η εφαρμογή '00000005-0000-0ff1-ce00-00000000000'(Yammer) είναι απενεργοποιημένη", υπάρχει ένα ζήτημα με την αρχή υπηρεσίας στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="72b30-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="72b30-104">Ένας διαχειριστής μπορεί να έχει απενεργοποιήσει την αρχή της υπηρεσίας για να αποκλείσει την πρόσβαση στο Yammer.</span><span class="sxs-lookup"><span data-stu-id="72b30-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="72b30-105">Η απενεργοποίηση της αρχής υπηρεσίας δεν συνιστάται και μπορεί να προκαλέσει πρόσθετα ζητήματα.</span><span class="sxs-lookup"><span data-stu-id="72b30-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="72b30-106">Για περισσότερες πληροφορίες σχετικά με την υποστηριζόμενη προσέγγιση για τον αποκλεισμό της πρόσβασης των χρηστών στο Yammer, ανατρέξτε στο θέμα [Απενεργοποίηση της πρόσβασης του Yammer για χρήστες της Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="72b30-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="72b30-107">Για να διορθώσετε αυτό το ζήτημα στην πύλη Azure και να επαναφέρετε την πρόσβαση χρήστη στο Yammer:</span><span class="sxs-lookup"><span data-stu-id="72b30-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="72b30-108">Ανοίξτε τη σελίδα Azure Active Directory και επιλέξτε **Εταιρικές εφαρμογές** στην περιοχή **Διαχείριση** στο αριστερό παράθυρο περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="72b30-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="72b30-109">Πληκτρολογήστε **Office 365 Yammer** στο πλαίσιο αναζήτησης και επιλέξτε το όνομα της εφαρμογής για να ανοίξετε τις ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="72b30-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="72b30-110">Επιλέξτε **Ιδιότητες** στην περιοχή **Διαχείριση** στο αριστερό παράθυρο περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="72b30-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="72b30-111">Ορίστε την τιμή **ενεργοποίησης για είσοδο των χρηστών; σε** **Ναι**και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="72b30-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="72b30-112">Πραγματοποιήστε ξανά είσοδο στο Yammer.</span><span class="sxs-lookup"><span data-stu-id="72b30-112">Sign in to Yammer again.</span></span> <span data-ttu-id="72b30-113">Ίσως χρειαστεί να καθαρίσετε τα cookies.</span><span class="sxs-lookup"><span data-stu-id="72b30-113">You might need to clear cookies.</span></span>

<span data-ttu-id="72b30-114">Εναλλακτικά, εκτελέστε εντολές PowerShell για να ορίσετε την τιμή.</span><span class="sxs-lookup"><span data-stu-id="72b30-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="72b30-115">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Λυπούμαστε, αλλά δεν αντιμετωπίζετε προβλήματα με την υπογραφή σας" όταν κάνετε κλικ στο πλακίδιο Yammer στο Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="72b30-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 