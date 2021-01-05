---
title: Πώς μπορείτε να προσθέσετε και να διαχειριστείτε διαχειριστές
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755495"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="7d6b4-102">Πώς μπορείτε να προσθέσετε και να διαχειριστείτε διαχειριστές</span><span class="sxs-lookup"><span data-stu-id="7d6b4-102">How to add and manage admins</span></span>

<span data-ttu-id="7d6b4-103">Με βάση την περιγραφή του ζητήματος, βρήκαμε μια λύση για εσάς.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="7d6b4-104">Οι περισσότεροι πελάτες μπόρεσαν να επιλύσουν το ζήτημά τους μόνοι τους, αφού ακολούθησαν την τεκμηρίωσή τους.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="7d6b4-105">Για να διαχειριστείτε το λογαριασμό χρέωσής σας για μια συμφωνία πελατών της Microsoft (MCA), μπορείτε να χρησιμοποιήσετε διαφορετικούς ρόλους με το επιθυμητό επίπεδο πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="7d6b4-106">Αυτοί οι ρόλοι είναι εκτός από τους ενσωματωμένους ρόλους υπηρεσίας Azure που σας βοηθούν να ελέγχετε τους πόρους σας.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="7d6b4-107">**Για να προσθέσετε ρόλους χρέωσης στην πύλη Azure:**</span><span class="sxs-lookup"><span data-stu-id="7d6b4-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="7d6b4-108">Πραγματοποιήστε είσοδο στην [πύλη Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7d6b4-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="7d6b4-109">Αναζητήστε *Διαχείριση κόστους + χρέωση*.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="7d6b4-110">Επιλέξτε Έλεγχος πρόσβασης (IAM) σε μια εμβέλεια, όπως το λογαριασμό χρέωσης, το προφίλ χρέωσης ή την ενότητα τιμολογίου όπου θέλετε να παράσχετε πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="7d6b4-111">Η σελίδα "Έλεγχος πρόσβασης (IAM)" παραθέτει τους χρήστες και τις ομάδες που έχουν ανατεθεί σε κάθε ρόλο για το συγκεκριμένο πεδίο.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="7d6b4-112">Για να παραχωρήσετε πρόσβαση σε ένα χρήστη, επιλέξτε **Προσθήκη** από το επάνω μέρος της σελίδας.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="7d6b4-113">Στην αναπτυσσόμενη λίστα *ρόλος* , επιλέξτε ένα ρόλο.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="7d6b4-114">Πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη στον οποίο θέλετε να δώσετε πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="7d6b4-115">Επιλέξτε **Αποθήκευση** για να εκχωρήσετε το ρόλο.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="7d6b4-116">Για να καταργήσετε την πρόσβαση για ένα χρήστη, επιλέξτε το χρήστη με την ανάθεση ρόλου που θέλετε να καταργήσετε.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="7d6b4-117">Επιλέξτε **Κατάργηση**.</span><span class="sxs-lookup"><span data-stu-id="7d6b4-117">Select **Remove**.</span></span>

<span data-ttu-id="7d6b4-118">**Προτεινόμενα έγγραφα**</span><span class="sxs-lookup"><span data-stu-id="7d6b4-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="7d6b4-119">Ορισμοί ρόλων χρέωσης</span><span class="sxs-lookup"><span data-stu-id="7d6b4-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="7d6b4-120">Ρόλοι και εργασίες λογαριασμού χρέωσης</span><span class="sxs-lookup"><span data-stu-id="7d6b4-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="7d6b4-121">Γρήγορα αποτελέσματα με το λογαριασμό χρέωσης MCA</span><span class="sxs-lookup"><span data-stu-id="7d6b4-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="7d6b4-122">Επιλέξτε πρόσβαση σε συμφωνία πελατών της Microsoft</span><span class="sxs-lookup"><span data-stu-id="7d6b4-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
