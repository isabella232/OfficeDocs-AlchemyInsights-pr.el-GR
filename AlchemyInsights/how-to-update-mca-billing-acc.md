---
title: Ενημέρωση σχετικά με την πώληση και τη διεύθυνση τιμολόγησης που σχετίζονται με τα βήματα που συνιστώνται για την MCA
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678478"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="851dc-102">Ενημέρωση σχετικά με την πώληση και τη διεύθυνση τιμολόγησης που σχετίζονται με τα βήματα που συνιστώνται για την MCA</span><span class="sxs-lookup"><span data-stu-id="851dc-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="851dc-103">Μπορείτε να ενημερώσετε τη διεύθυνση πώλησης και τιμολόγησης που είναι συσχετισμένη με τη συμφωνία πελατών της Microsoft (MCA).</span><span class="sxs-lookup"><span data-stu-id="851dc-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="851dc-104">Μόνο ένας διαχειριστής χρήστη μπορεί να κάνει αλλαγές στις πληροφορίες προφίλ χρήστη του Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="851dc-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="851dc-105">Εάν δεν σας έχει εκχωρηθεί ο ρόλος διαχειριστή χρήστη, επικοινωνήστε με το διαχειριστή χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="851dc-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="851dc-106">Για περισσότερες πληροφορίες σχετικά με την αλλαγή του προφίλ ενός χρήστη, ανατρέξτε στο θέμα [Προσθήκη ή ενημέρωση των πληροφοριών προφίλ ενός χρήστη με χρήση του Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="851dc-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="851dc-107">**Διεύθυνση πώλησης** -η διεύθυνση πώλησης είναι η διεύθυνση και τα στοιχεία επικοινωνίας του οργανισμού ή του ατόμου, ο οποίος είναι υπεύθυνος για ένα λογαριασμό χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="851dc-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="851dc-108">Εμφανίζεται σε όλα τα τιμολόγια που δημιουργούνται για το λογαριασμό χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="851dc-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="851dc-109">**Διεύθυνση τιμολόγησης** -η διεύθυνση τιμολόγησης είναι η διεύθυνση και τα στοιχεία επικοινωνίας του οργανισμού ή του ατόμου, ο οποίος είναι υπεύθυνος για τα τιμολόγια που δημιουργούνται για ένα λογαριασμό χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="851dc-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="851dc-110">Για ένα λογαριασμό χρέωσης για μια MCA, υπάρχει μια διεύθυνση τιμολόγησης για κάθε προφίλ χρέωσης και εμφανίζεται στο τιμολόγιο που έχει δημιουργηθεί για το προφίλ χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="851dc-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="851dc-111">**Για να ενημερώσετε έναν λογαριασμό τιμολόγησης MCA που πωλείται σε διεύθυνση**:</span><span class="sxs-lookup"><span data-stu-id="851dc-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="851dc-112">Πραγματοποιήστε είσοδο στην πύλη Azure χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου, η οποία έχει έναν κάτοχο ή ένα ρόλο συμβολής στο λογαριασμό χρέωσης για μια MCA.</span><span class="sxs-lookup"><span data-stu-id="851dc-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="851dc-113">Αναζητήστε χρεώσεις **διαχείρισης κόστους**  +  .</span><span class="sxs-lookup"><span data-stu-id="851dc-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="851dc-114">Κάντε κλικ στην επιλογή **Ιδιότητες**  >  **ενημέρωσης sold-To**.</span><span class="sxs-lookup"><span data-stu-id="851dc-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="851dc-115">Πληκτρολογήστε τη νέα διεύθυνση και κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="851dc-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="851dc-116">Ορισμένοι λογαριασμοί απαιτούν επιπλέον επαλήθευση πριν από την ενημέρωση της διεύθυνσης πώλησης.</span><span class="sxs-lookup"><span data-stu-id="851dc-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="851dc-117">Εάν ο λογαριασμός σας απαιτεί μη αυτόματη έγκριση, θα σας ζητηθεί να επικοινωνήσετε με την υποστήριξη Azure.</span><span class="sxs-lookup"><span data-stu-id="851dc-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="851dc-118">**Για να ενημερώσετε μια διεύθυνση λογαριασμού ΧΡΈΩΣΗς MCA**:</span><span class="sxs-lookup"><span data-stu-id="851dc-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="851dc-119">Πραγματοποιήστε είσοδο στην πύλη Azure χρησιμοποιώντας τη διεύθυνση ηλεκτρονικού ταχυδρομείου, η οποία έχει έναν κάτοχο ή ένα ρόλο συμβολής σε ένα λογαριασμό χρέωσης ή ένα προφίλ χρέωσης για μια MCA.</span><span class="sxs-lookup"><span data-stu-id="851dc-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="851dc-120">Αναζητήστε χρεώσεις **διαχείρισης κόστους**  +  .</span><span class="sxs-lookup"><span data-stu-id="851dc-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="851dc-121">Επιλέξτε **προφίλ χρέωσης** και επιλέξτε ένα προφίλ χρέωσης για να ενημερώσετε τη διεύθυνση χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="851dc-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="851dc-122">Κάντε κλικ στην επιλογή  >  **διεύθυνση ενημέρωσης** ιδιοτήτων.</span><span class="sxs-lookup"><span data-stu-id="851dc-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="851dc-123">Πληκτρολογήστε τη νέα διεύθυνση και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="851dc-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="851dc-124">**Προτεινόμενα έγγραφα**</span><span class="sxs-lookup"><span data-stu-id="851dc-124">**Recommended documents**</span></span>

<span data-ttu-id="851dc-125">[Αλλαγή των στοιχείων επικοινωνίας για ένα λογαριασμό χρέωσης Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="851dc-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="851dc-126">Ενημέρωση ρυθμίσεων λογαριασμού χρέωσης</span><span class="sxs-lookup"><span data-stu-id="851dc-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="851dc-127">Κατανόηση των ρόλων διαχείρισης της συμφωνίας πελατών της Microsoft στο Azure</span><span class="sxs-lookup"><span data-stu-id="851dc-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)