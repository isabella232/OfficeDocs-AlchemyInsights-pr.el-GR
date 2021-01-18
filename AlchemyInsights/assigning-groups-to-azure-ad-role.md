---
title: Αντιστοίχιση ομάδων σε ρόλο AD Azure
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885066"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="a91a9-102">Αντιστοίχιση ομάδων σε ρόλο AD Azure</span><span class="sxs-lookup"><span data-stu-id="a91a9-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="a91a9-103">Για να αντιστοιχίσετε μια ομάδα AD Azure με την προέλευση της αρχής στο Azure AD σε ένα ρόλο Azure AD, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="a91a9-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="a91a9-104">Δημιουργία νέας ομάδας-για να δημιουργήσετε μια νέα ομάδα:</span><span class="sxs-lookup"><span data-stu-id="a91a9-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="a91a9-105">a.</span><span class="sxs-lookup"><span data-stu-id="a91a9-105">a.</span></span> <span data-ttu-id="a91a9-106">Πραγματοποιήστε είσοδο στο κέντρο διαχείρισης Azure AD με δικαιώματα διαχειριστή με δικαιώματα **διαχειριστή** ή **καθολικά δικαιώματα διαχειριστή** .</span><span class="sxs-lookup"><span data-stu-id="a91a9-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="a91a9-107">b.</span><span class="sxs-lookup"><span data-stu-id="a91a9-107">b.</span></span> <span data-ttu-id="a91a9-108">Επιλέξτε **> ομάδες Azure Active Directory > όλες τις ομάδες > νέα ομάδα**.</span><span class="sxs-lookup"><span data-stu-id="a91a9-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="a91a9-109">c.</span><span class="sxs-lookup"><span data-stu-id="a91a9-109">c.</span></span> <span data-ttu-id="a91a9-110">Δημιουργήστε την ομάδα.</span><span class="sxs-lookup"><span data-stu-id="a91a9-110">Create the group.</span></span>

2. <span data-ttu-id="a91a9-111">Εκχωρήστε το ρόλο στην ομάδα κατά τη δημιουργία ομάδας ή μετά τη δημιουργία της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="a91a9-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="a91a9-112">a.</span><span class="sxs-lookup"><span data-stu-id="a91a9-112">a.</span></span> <span data-ttu-id="a91a9-113">Για να αντιστοιχίσετε ένα ρόλο στην ομάδα τη στιγμή της δημιουργίας της ομάδας, ενεργοποιήστε την εναλλαγή **ρόλων AD Azure μπορούν να εκχωρηθούν στην ομάδα** και να δημιουργήσετε την ομάδα.</span><span class="sxs-lookup"><span data-stu-id="a91a9-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="a91a9-114">b.</span><span class="sxs-lookup"><span data-stu-id="a91a9-114">b.</span></span> <span data-ttu-id="a91a9-115">Για να αντιστοιχίσετε ένα ρόλο στην ομάδα μετά τη δημιουργία της, μεταβείτε στην καρτέλα **αντιστοιχισμένοι ρόλοι** για την ομάδα που μόλις δημιουργήσατε και αντιστοιχίστε το ρόλο στην ομάδα.</span><span class="sxs-lookup"><span data-stu-id="a91a9-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="a91a9-116">**Διαχείριση ιδιότητας μέλους μιας ομάδας που έχει αντιστοιχιστεί σε ρόλο AD Azure**</span><span class="sxs-lookup"><span data-stu-id="a91a9-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="a91a9-117">Για να αποτρέψετε την ανύψωση δικαιωμάτων, από προεπιλογή, μόνο οι διαχειριστές με δικαιώματα ρόλου και οι Καθολικοί διαχειριστές μπορούν να τροποποιήσουν τη συμμετοχή σε μια ομάδα που έχει εκχωρηθεί σε ένα ρόλο.</span><span class="sxs-lookup"><span data-stu-id="a91a9-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="a91a9-118">Ωστόσο, μπορούν να επιλέξουν να εκχωρήσουν έναν κάτοχο για μια τέτοια ομάδα και να αναθέσουν αυτή την εργασία.</span><span class="sxs-lookup"><span data-stu-id="a91a9-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="a91a9-119">Για περισσότερες λεπτομέρειες σχετικά με την εκχώρηση ομάδων cloud σε ρόλους AD Azure, ανατρέξτε στο θέμα [Εκχώρηση ρόλων διαφήμισης σε ομάδα cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="a91a9-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="a91a9-120">Για περισσότερες λεπτομέρειες σχετικά με την αντιμετώπιση προβλημάτων που έχουν εκχωρηθεί σε ομάδες cloud, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων που έχουν εκχωρηθεί σε ομάδες cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="a91a9-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





