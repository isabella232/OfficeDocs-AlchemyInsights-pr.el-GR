---
title: Συγχρονισμός υπηρεσίας τομέα
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885157"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="6afb2-102">Συγχρονισμός υπηρεσίας τομέα</span><span class="sxs-lookup"><span data-stu-id="6afb2-102">Domain service synchronization</span></span>

<span data-ttu-id="6afb2-103">Τα αντικείμενα και τα διαπιστευτήρια σε έναν διαχειριζόμενο τομέα των υπηρεσιών τομέα Azure Active Directory (Azure AD DS) μπορούν να δημιουργηθούν τοπικά μέσα στον τομέα ή να συγχρονιστούν από έναν μισθωτή του Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6afb2-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="6afb2-104">Όταν αναπτύσσετε για πρώτη φορά το Azure AD DS, ένας αυτόματος μονόδρομος συγχρονισμός έχει ρυθμιστεί και ξεκινά για την αναπαραγωγή των αντικειμένων από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6afb2-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="6afb2-105">Αυτός ο μονόδρομος συγχρονισμός εξακολουθεί να εκτελείται στο παρασκήνιο για να διατηρεί τον τομέα διαχείρισης του Azure AD DS ενημερωμένο με τυχόν αλλαγές από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6afb2-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="6afb2-106">Δεν γίνεται συγχρονισμός από το Azure AD DS ξανά στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6afb2-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="6afb2-107">Για περισσότερες λεπτομέρειες σχετικά με το συγχρονισμό υπηρεσίας τομέα του Azure Active Directory, ανατρέξτε στο θέμα [Συγχρονισμός υπηρεσίας τομέα](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="6afb2-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
