---
title: Διαγραφή μισθωτή
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564621"
---
# <a name="delete-tenant"></a><span data-ttu-id="b15db-102">Διαγραφή μισθωτή</span><span class="sxs-lookup"><span data-stu-id="b15db-102">Delete tenant</span></span>

<span data-ttu-id="b15db-103">Για να διαγράψετε μια AD Azure, βεβαιωθείτε ότι:</span><span class="sxs-lookup"><span data-stu-id="b15db-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="b15db-104">Είστε καθολικός διαχειριστής στον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="b15db-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="b15db-105">Δεν έχετε εισέλθει με ένα λογαριασμό που έχει τον προεπιλεγμένο κατάλογο, όπως το contoso.onmicrosoft.com στο λογαριασμό που έχει υπογραφεί, όπως το admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="b15db-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="b15db-106">Καταργήστε τυχόν ενεργές εφαρμογές στον κατάλογο πριν από τη διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="b15db-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="b15db-107">Για να καταργήσετε τις ενεργές εφαρμογές, μεταβείτε στις καταχωρήσεις εφαρμογών και καταργήστε τις υπάρχουσες εφαρμογές.</span><span class="sxs-lookup"><span data-stu-id="b15db-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="b15db-108">Δεν υπάρχουν ενεργές συνδρομές για οποιαδήποτε Microsoft Online Services, όπως το Microsoft Azure, το Office 365 ή το Azure AD Premium που σχετίζεται με τον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="b15db-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="b15db-109">Μεταφέρετε τις συνδρομές σας ή επιταχύνετε την ακύρωση των ενεργών συνδρομών μέσω υποστήριξης Azure και χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="b15db-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="b15db-110">Μάθετε περισσότερα σχετικά με το πώς μπορείτε να ακυρώσετε τις συνδρομές του Office 365 και του Azure.</span><span class="sxs-lookup"><span data-stu-id="b15db-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="b15db-111">Για οδηγίες σχετικά με τη συσχέτιση ή την προσθήκη μιας υπάρχουσας συνδρομής σε έναν μισθωτή, ανατρέξτε στο θέμα [συσχέτιση ή προσθήκη μιας συνδρομής Azure στον ΜΙΣΘΩΤΉ AD Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="b15db-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="b15db-112">Δεν υπάρχει ενεργή άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="b15db-112">There are no Active license.</span></span> <span data-ttu-id="b15db-113">Για να καταργήσετε άδειες χρήσης, ανατρέξτε στο θέμα [Πώς να καταργήσετε τη συνδρομή για να καταργήσετε την άδεια χρήσης](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="b15db-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="b15db-114">Δεν υπάρχουν άλλοι ενεργοί χρήστες στον κατάλογο εκτός από εσάς ως καθολικός διαχειριστής, όταν προσπαθείτε να διαγράψετε το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b15db-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="b15db-115">Καταργήστε τυχόν άλλους ενεργούς χρήστες και οποιεσδήποτε εξαρτήσεις σε ένα προσαρμοσμένο όνομα τομέα στον μισθωτή θα πρέπει επίσης να καταργηθούν, όπως οι χρήστες που έχουν δημιουργηθεί με το admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b15db-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="b15db-116">Για περισσότερες λεπτομέρειες, μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="b15db-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="b15db-117">Διαγράψτε τη φράση "Azure Active Directory" ή "συνδρομή", ανατρέξτε στο θέμα [Διαγραφή υπηρεσίας καταλόγου Active Directory Azure](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="b15db-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="b15db-118">Κατάργηση εφαρμογών στον κατάλογο, ανατρέξτε στο θέμα [Κατάργηση εφαρμογών](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="b15db-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
