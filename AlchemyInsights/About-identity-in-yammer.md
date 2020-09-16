---
title: Πληροφορίες για την ταυτότητα στο Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664170"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="2b27b-102">Πληροφορίες για την ταυτότητα στο Yammer</span><span class="sxs-lookup"><span data-stu-id="2b27b-102">About identity in Yammer</span></span>

<span data-ttu-id="2b27b-103">Συνιστάται όλα τα δίκτυα να ακολουθούν τα παρακάτω βήματα για την αποφυγή προβλημάτων που σχετίζονται με την ταυτότητα:</span><span class="sxs-lookup"><span data-stu-id="2b27b-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="2b27b-104">Επιβολή ταυτότητας του Office 365 μετά την προμήθεια λογαριασμών του Microsoft 365 για τους χρήστες στο Azure AD για να εξασφαλίσετε ότι όλοι οι χρήστες θα εισέλθετε χρησιμοποιώντας τον κύριο λογαριασμό τους Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b27b-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="2b27b-105">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα επιβολή ταυτότητας του Office 365 για τους χρήστες του Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="2b27b-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="2b27b-106">Εδραίωση πολλών δικτύων Yammer.</span><span class="sxs-lookup"><span data-stu-id="2b27b-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="2b27b-107">Οι ρυθμίσεις παραμέτρων Yammer παλαιού τύπου επιτρέπουν τη σύνδεση πολλών δικτύων Yammer με έναν μισθωτή.</span><span class="sxs-lookup"><span data-stu-id="2b27b-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="2b27b-108">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα μετεγκατάσταση δικτύου-εδραίωση πολλών δικτύων Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="2b27b-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="2b27b-109">Προαιρετικά, επιβάλετε την άδεια χρήσης για το Yammer για να αποκλείσετε χρήστες από το Yammer, εάν δεν διαθέτουν άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="2b27b-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="2b27b-110">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Διαχείριση αδειών χρήσης του Yammer στο Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2b27b-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="2b27b-111">Τέλος, ελέγξτε τη λίστα χρηστών για παλαιότερα δίκτυα Yammer και αναστείλετε παλαιούς χρήστες.</span><span class="sxs-lookup"><span data-stu-id="2b27b-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="2b27b-112">Συνιστάται να αναστείλετε (να απενεργοποιήσετε) τους χρήστες αντί να τους διαγράψετε, επειδή η διαγραφή είναι μη αναστρέψιμη.</span><span class="sxs-lookup"><span data-stu-id="2b27b-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="2b27b-113">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Έλεγχος χρηστών του Yammer σε δίκτυα που είναι συνδεδεμένα με το Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) και [Κατάργηση χρηστών](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="2b27b-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="2b27b-114">Με τη ρύθμιση παραμέτρων του Yammer χρησιμοποιώντας αυτά τα βήματα, θα είστε επίσης έτοιμοι να ρυθμίσετε τις παραμέτρους του δικτύου Yammer για εγγενή λειτουργία για το Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b27b-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="2b27b-115">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Ρύθμιση παραμέτρων του δικτύου Yammer για εγγενή λειτουργία για το Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="2b27b-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>