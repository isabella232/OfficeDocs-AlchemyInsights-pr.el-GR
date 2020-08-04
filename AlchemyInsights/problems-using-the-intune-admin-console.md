---
title: Προβλήματα με τη χρήση της κονσόλας διαχείρισης Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555039"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="4487e-102">Προβλήματα με τη χρήση της κονσόλας διαχείρισης Intune</span><span class="sxs-lookup"><span data-stu-id="4487e-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="4487e-103">**"Δεν επιτρέπεται η πρόσβαση" κατά την περιήγηση στην πύλη διαχείρισης Intune.**</span><span class="sxs-lookup"><span data-stu-id="4487e-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="4487e-104">Εάν είστε μέλος ενός προσαρμοσμένου ρόλου Intune, βεβαιωθείτε ότι έχει εκχωρηθεί στο λογαριασμό σας μια άδεια χρήσης Intune ή Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="4487e-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="4487e-105">Εάν χρησιμοποιείτε τη Διαχείριση ρύθμισης παραμέτρων για τη διαχείριση συσκευών, βεβαιωθείτε ότι δεν είστε μέρος της συλλογής χρηστών Intune για το MDM της Διαχείρισης ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="4487e-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="4487e-106">Βεβαιωθείτε ότι σας έχουν εκχωρηθεί τα κατάλληλα δικαιώματα ελέγχου διαχείρισης που βασίζονται σε ρόλους (RBAC) στη λεπίδα ρόλων Intune.</span><span class="sxs-lookup"><span data-stu-id="4487e-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="4487e-107">Βεβαιωθείτε ότι η ομάδα που χρησιμοποιείται δεν είναι λίστα διανομής.</span><span class="sxs-lookup"><span data-stu-id="4487e-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="4487e-108">Το Intune στην πύλη Azure υποστηρίζει μόνο λογαριασμούς χρηστών που ανήκουν σε ομάδες ασφαλείας της υπηρεσίας καταλόγου Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="4487e-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="4487e-109">Εξετάστε τις ομάδες σας στην πύλη Azure > ομάδες **Intune**  >  **Groups**ή στην πύλη Azure > υπηρεσία καταλόγου Azure **Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="4487e-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="4487e-110">**Ο χρήστης έχει πάρα πολλά δικαιώματα για το ρόλο Intune που έχει εκχωρηθεί**</span><span class="sxs-lookup"><span data-stu-id="4487e-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="4487e-111">Συμβουλέψτε το χρήστη να μεταβεί **στους ρόλους Intune**  >  **Intune**  >  **Τα δικαιώματά μου**  >  **Εξαγωγή** για να αναθεωρήσετε τα εκχωρημένα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="4487e-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="4487e-112">**Πρόσθεσα μια ομάδα εμβέλειας σε ένα ρόλο, αλλά οι χρήστες σε αυτόν το ρόλο εξακολουθούν να βλέπουν άλλους χρήστες ή συσκευές.**</span><span class="sxs-lookup"><span data-stu-id="4487e-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="4487e-113">Οι ομάδες εμβέλειας δεν φιλτράρουν χρήστες ή συσκευές.</span><span class="sxs-lookup"><span data-stu-id="4487e-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="4487e-114">Ομάδες εμβέλειας:</span><span class="sxs-lookup"><span data-stu-id="4487e-114">Scope groups:</span></span>

- <span data-ttu-id="4487e-115">Περιορίστε σε ποιους χρήστες μπορούν να εκχωρήσουν πολιτικές ή εφαρμογές.</span><span class="sxs-lookup"><span data-stu-id="4487e-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="4487e-116">Να επιτρέπεται μόνο σε συγκεκριμένους χρήστες να εκτελούν απομακρυσμένες εργασίες σε συσκευές.</span><span class="sxs-lookup"><span data-stu-id="4487e-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="4487e-117">Για περισσότερες πληροφορίες σχετικά με τις ομάδες εμβέλειας, ανατρέξτε στο θέμα [Έλεγχος πρόσβασης βάσει ρόλων (RBAC) με το Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="4487e-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4487e-118">**Πρόσθεσα ένα χρήστη σε ένα ρόλο Intune, αλλά εξακολουθούν να έχουν πλήρη πρόσβαση στην κονσόλα admin Intune.**</span><span class="sxs-lookup"><span data-stu-id="4487e-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="4487e-119">Μεταβείτε στο Intune > **χρήστες** στην πύλη Azure και βεβαιωθείτε ότι ο χρήστης δεν έχει αντιστοιχιστεί σε κανέναν από τους ακόλουθους ρόλους στην πύλη Azure:</span><span class="sxs-lookup"><span data-stu-id="4487e-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="4487e-120">Καθολικός διαχειριστής</span><span class="sxs-lookup"><span data-stu-id="4487e-120">Global administrator</span></span>
- <span data-ttu-id="4487e-121">Διαχειριστής υπηρεσίας Intune</span><span class="sxs-lookup"><span data-stu-id="4487e-121">Intune service administrator</span></span>
- <span data-ttu-id="4487e-122">Διαχειριστής του SharePoint</span><span class="sxs-lookup"><span data-stu-id="4487e-122">SharePoint administrator</span></span>

<span data-ttu-id="4487e-123">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Έλεγχος πρόσβασης βάσει ρόλων (RBAC) με το Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="4487e-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4487e-124">**Θέματα πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="4487e-124">**Access Issues**</span></span>

<span data-ttu-id="4487e-125">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δεν μπορείτε να εισέλθετε στο Office 365, azure ή Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="4487e-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>