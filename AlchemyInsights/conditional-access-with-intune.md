---
title: Υπό όρους πρόσβασης με Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290467"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0e56f-102">Υπό όρους πρόσβασης με Intune</span><span class="sxs-lookup"><span data-stu-id="0e56f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0e56f-103">Χρήση **Υπό όρους πρόσβασης** με Intune απαιτεί τρία βήματα:</span><span class="sxs-lookup"><span data-stu-id="0e56f-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="0e56f-p101">Για να δημιουργήσετε μια **Πολιτική υπό όρους πρόσβασης** , η οποία ορίζει τους πόρους που προστατεύονται και τι συνθήκες πρέπει να τηρούνται για να αποκτήσετε πρόσβαση σε αυτούς τους πόρους. Για παράδειγμα, μια συσκευή πρέπει να είναι συμβατή με πριν από την πρόσβαση σε εταιρικό μήνυμα ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="0e56f-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="0e56f-p102">Δημιουργία **Πολιτικής συμμόρφωσης** για να καθορίσετε τις ρυθμίσεις που πρέπει να πληρούνται προτού θεωρηθεί συμβατό με τη συσκευή. Για παράδειγμα, μια συσκευή πρέπει να έχει τουλάχιστον 6 ψηφίων pin πριν να θεωρείται συμβατή με.</span><span class="sxs-lookup"><span data-stu-id="0e56f-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="0e56f-p103">Διασφάλιση της **Συμμόρφωσης πολιτικές** και **Πολιτικές υπό όρους πρόσβασης** που προορίζονται για την επιθυμητή ομάδες χρηστών. Αυτό μπορεί να απαιτεί τη δημιουργία συγκεκριμένων ομάδων χρηστών στον κατάλογο Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="0e56f-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="0e56f-110">Περισσότερες πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="0e56f-110">Read more:</span></span>
  
- [<span data-ttu-id="0e56f-111">Βέλτιστες πρακτικές υπό όρους πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="0e56f-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="0e56f-112">Γρήγορα αποτελέσματα με την υπό όρους πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="0e56f-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

