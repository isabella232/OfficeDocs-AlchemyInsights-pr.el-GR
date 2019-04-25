---
title: Υπό όρους πρόσβασης με Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393541"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="1b90d-102">Υπό όρους πρόσβασης με Intune</span><span class="sxs-lookup"><span data-stu-id="1b90d-102">Conditional Access with Intune</span></span>

<span data-ttu-id="1b90d-103">Χρήση **Υπό όρους πρόσβασης** με Intune απαιτεί τρία βήματα:</span><span class="sxs-lookup"><span data-stu-id="1b90d-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="1b90d-104">Για να δημιουργήσετε μια **Πολιτική υπό όρους πρόσβασης** , η οποία ορίζει τους πόρους που προστατεύονται και τι συνθήκες πρέπει να τηρούνται για να αποκτήσετε πρόσβαση σε αυτούς τους πόρους.</span><span class="sxs-lookup"><span data-stu-id="1b90d-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="1b90d-105">Για παράδειγμα, μια συσκευή πρέπει να είναι συμβατή με πριν από την πρόσβαση σε εταιρικό μήνυμα ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="1b90d-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="1b90d-106">Δημιουργία **Πολιτικής συμμόρφωσης** για να καθορίσετε τις ρυθμίσεις που πρέπει να πληρούνται προτού θεωρηθεί συμβατό με τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="1b90d-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="1b90d-107">Για παράδειγμα, μια συσκευή πρέπει να έχει τουλάχιστον 6 ψηφίων pin πριν να θεωρείται συμβατή με.</span><span class="sxs-lookup"><span data-stu-id="1b90d-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="1b90d-108">Διασφάλιση της **Συμμόρφωσης πολιτικές** και **Πολιτικές υπό όρους πρόσβασης** που προορίζονται για την επιθυμητή ομάδες χρηστών.</span><span class="sxs-lookup"><span data-stu-id="1b90d-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="1b90d-109">Αυτό μπορεί να απαιτεί τη δημιουργία συγκεκριμένων ομάδων χρηστών στον κατάλογο Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="1b90d-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="1b90d-110">Περισσότερες πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="1b90d-110">Read more:</span></span>
  
- [<span data-ttu-id="1b90d-111">Βέλτιστες πρακτικές υπό όρους πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="1b90d-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="1b90d-112">Γρήγορα αποτελέσματα με την υπό όρους πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="1b90d-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

