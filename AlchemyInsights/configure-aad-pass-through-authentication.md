---
title: Ρύθμιση παραμέτρων του ελέγχου ταυτότητας πρόσβασης του Azure Active Directory
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036295"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="4e05c-102">Ρύθμιση παραμέτρων του ελέγχου ταυτότητας πρόσβασης του Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4e05c-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="4e05c-103">Ακολουθούν ορισμένοι οδηγοί που θα σας βοηθήσουν να ρυθμίσετε τις παραμέτρους του ελέγχου ταυτότητας μέσω πρόσβασης:</span><span class="sxs-lookup"><span data-stu-id="4e05c-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="4e05c-104">**Για να ρυθμίσετε το Azure Active Directory Connect:** Οι χρήστες συγχρονισμού στον οδηγό καταλόγου σάς βοηθούν να ρυθμίσετε τις παραμέτρους του συγχρονισμού του hash κωδικού πρόσβασης ή του ελέγχου ταυτότητας πρόσβασης. [](https://admin.microsoft.com/AdminPortal/Home)</span><span class="sxs-lookup"><span data-stu-id="4e05c-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="4e05c-105">Αυτή η ρύθμιση παραμέτρων επιτρέπει στους χρήστες να πραγματοποιήσουν είσοδο στο ηλεκτρονικό ταχυδρομείο τους και στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης (ελεγκτής τομέα) χρησιμοποιώντας τον ίδιο κωδικό πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="4e05c-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="4e05c-106">Ο [οδηγός συγχρονισμού χρηστών στον οδηγό](https://admin.microsoft.com/AdminPortal/Home) καταλόγου καλύπτει επίσης την είσοδο ομοσπονδίας με τις υπηρεσίες Active Directory Federation Services (AD FS).</span><span class="sxs-lookup"><span data-stu-id="4e05c-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="4e05c-107">**Για** να ρυθμίσετε τις δυνατότητες του [Azure:](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) Ο οδηγός ρύθμισης του Azure AD σάς καθοδηγεί στη ρύθμιση των δυνατοτήτων του Azure Active Directory Basic, όπως η διαχείριση πρόσβασης βάσει ομάδας, η επαναφορά κωδικού πρόσβασης από το χρήστη για εφαρμογές cloud και ο διακομιστής μεσολάβησης εφαρμογών Azure Active Directory για τη δημοσίευση εφαρμογών web εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="4e05c-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


