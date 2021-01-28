---
title: Ζητήματα παροχής από τους χρήστες
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7762"
- "9004348"
ms.openlocfilehash: eed5886e5de391a203882f373f7ba8a71830b0d1
ms.sourcegitcommit: 28a79ef23c4a510397f4a8339ac2c5ff70eec713
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50035925"
---
# <a name="user-provisioning-issues"></a><span data-ttu-id="f24af-102">Ζητήματα παροχής χρηστών</span><span class="sxs-lookup"><span data-stu-id="f24af-102">User-provisioning issues</span></span>

<span data-ttu-id="f24af-103">Αυτό το άρθρο περιγράφει τον τρόπο αντιμετώπισης προβλημάτων που αντιμετωπίζετε κατά την προμήθεια χρηστών.</span><span class="sxs-lookup"><span data-stu-id="f24af-103">This article describes how to troubleshoot the issues you face when provisioning users.</span></span>

<span data-ttu-id="f24af-104">Για οδηγίες όταν αντιμετωπίζετε διάφορα ζητήματα παροχής από το χρήστη, ακολουθήστε τις παρακάτω οδηγίες:</span><span class="sxs-lookup"><span data-stu-id="f24af-104">For guidance when encountering the various user-provisioning issues, follow the instructions below:</span></span>

1. <span data-ttu-id="f24af-105">Θα πρέπει πάντα να ξεκινάτε βρίσκοντας το πρόγραμμα εκμάθησης ρύθμισης που αφορά τη ρύθμιση προμήθειας για την εφαρμογή σας.</span><span class="sxs-lookup"><span data-stu-id="f24af-105">You should always start by finding the setup tutorial specific to setting up provisioning for your application.</span></span> <span data-ttu-id="f24af-106">Στη συνέχεια, ακολουθήστε αυτά τα βήματα για να ρυθμίσετε τις παραμέτρους τόσο της εφαρμογής όσο και του Azure Active Directory (AD) για να δημιουργήσετε τη σύνδεση προμήθειας.</span><span class="sxs-lookup"><span data-stu-id="f24af-106">Then follow those steps to configure both the app and Azure Active Directory (AD) to create the provisioning connection.</span></span> <span data-ttu-id="f24af-107">Μπορείτε να βρείτε μια λίστα με προγράμματα εκμάθησης εφαρμογών στη λίστα με τα προγράμματα εκμάθησης σχετικά με τον τρόπο ενοποίησης [εφαρμογών SaaS με το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)</span><span class="sxs-lookup"><span data-stu-id="f24af-107">A list of app tutorials can be found at [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).</span></span>
2. <span data-ttu-id="f24af-108">Αντιμετωπίστε τα προβλήματα παροχής από τους χρήστες κάνοντας αναφορά στα ακόλουθα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="f24af-108">Troubleshoot the user-provisioning issues by referring to the following articles:</span></span>
    - <span data-ttu-id="f24af-109">[Γνωστά θέματα](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues) : Για να γνωρίζετε πότε εργάζεστε με προμήθεια εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="f24af-109">[Known issues](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues) - To be aware of when working with app provisioning.</span></span>
    - <span data-ttu-id="f24af-110">[Παροχή αναφορών](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) στην πύλη του Azure Active Directory (προεπισκόπηση)</span><span class="sxs-lookup"><span data-stu-id="f24af-110">[Provisioning reports](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in the Azure Active Directory portal (preview)</span></span>
    - [<span data-ttu-id="f24af-111">Δεν ξέρω πώς μπορείτε να ρυθμίσετε τις παραμέτρους προμήθειας χρήστη σε μια εφαρμογή azure AD Gallery</span><span class="sxs-lookup"><span data-stu-id="f24af-111">I don't know how to configure user provisioning to an Azure AD Gallery application</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/configure-automatic-user-provisioning-portal) 
    - [<span data-ttu-id="f24af-112">Παρουσιάστηκε πρόβλημα κατά τη ρύθμιση των παραμέτρων παροχής χρήστη σε μια εφαρμογή του Azure AD Gallery</span><span class="sxs-lookup"><span data-stu-id="f24af-112">I encountered a problem when configuring user provisioning to an Azure AD Gallery application</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem) 
    - [<span data-ttu-id="f24af-113">Έχω ρυθμίσει την προμήθεια στην εφαρμογή Azure AD Gallery, αλλά δεν γίνεται προμήθεια χρηστών</span><span class="sxs-lookup"><span data-stu-id="f24af-113">I've set up provisioning to my Azure AD Gallery application, but no users are being provisioned</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned) 
    - [<span data-ttu-id="f24af-114">Η προμήθεια στην εφαρμογή Azure AD Gallery λειτουργεί, αλλά γίνεται προμήθεια εσφαλμένου συνόλου χρηστών</span><span class="sxs-lookup"><span data-stu-id="f24af-114">Provisioning to my Azure AD Gallery application is working, but the wrong set of users are being provisioned</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-assign-users)





