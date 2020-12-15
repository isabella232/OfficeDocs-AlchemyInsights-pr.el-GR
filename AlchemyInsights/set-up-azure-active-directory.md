---
title: Ρύθμιση της υπηρεσίας καταλόγου Active Directory Azure
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
- "9004192"
- "7373"
ms.openlocfilehash: 94078246562112709eee303fa13d4ac2aa651b12
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678282"
---
# <a name="set-up-azure-active-directory"></a><span data-ttu-id="694c2-102">Ρύθμιση της υπηρεσίας καταλόγου Active Directory Azure</span><span class="sxs-lookup"><span data-stu-id="694c2-102">Set up Azure Active Directory</span></span>

<span data-ttu-id="694c2-103">Ο [Οδηγός εγκατάστασης του Azure AD](https://go.microsoft.com/fwlink/?linkid=2134390) παρέχει πληροφορίες για να εξασφαλίσει ότι η εταιρεία σας διαθέτει μια ισχυρή βάση ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="694c2-103">The [Azure AD setup guide](https://go.microsoft.com/fwlink/?linkid=2134390) provides information to ensure your organization has a strong security foundation.</span></span> <span data-ttu-id="694c2-104">Σε αυτόν τον οδηγό, θα ρυθμίσετε τις αρχικές δυνατότητες, όπως τον έλεγχο πρόσβασης που βασίζεται στο ρόλο του Azure (Azure RBAC) για διαχειριστές, το Azure AD Connect για τον κατάλογο εσωτερικής εγκατάστασης και την εύρυθμη λειτουργία του Azure AD Connect, ώστε να μπορείτε να παρακολουθείτε την υγεία της υβριδικής ταυτότητάς σας κατά τη διάρκεια αυτόματων συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="694c2-104">In this guide you will set up initial features, like Azure role-based access control (Azure RBAC) for admins, Azure AD Connect for your on-premises directory, and Azure AD Connect Health, so you can monitor your hybrid identity's health during automated syncs.</span></span>

<span data-ttu-id="694c2-105">Περιλαμβάνει επίσης βασικές πληροφορίες σχετικά με την ενεργοποίηση της λειτουργίας του κωδικού πρόσβασης από το χρήστη, της πρόσβασης υπό όρους και της ενσωματωμένης σύνδεσης τρίτου μέρους, συμπεριλαμβανομένης της προαιρετικής προηγμένης προστασίας ταυτότητας και του αυτοματισμού παροχής χρηστών.</span><span class="sxs-lookup"><span data-stu-id="694c2-105">It also includes essential information on enabling self-service password resets, conditional access and integrated third-party sign-on including optional advanced identity protection and user provisioning automation.</span></span>
