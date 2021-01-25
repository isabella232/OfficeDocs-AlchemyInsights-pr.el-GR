---
title: Αντιστοίχιση χαρακτηριστικού παροχής χρήστη
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
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949762"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="6f884-102">Αντιστοίχιση χαρακτηριστικού παροχής χρήστη</span><span class="sxs-lookup"><span data-stu-id="6f884-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="6f884-103">Για να αντιμετωπίσετε γνωστά προβλήματα αντιστοίχισης χαρακτηριστικών, ανατρέξτε στο θέμα [αντιστοιχίσεις χαρακτηριστικών](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="6f884-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="6f884-104">Ο Microsoft Azure Active Directory (AD) παρέχει υποστήριξη για την προμήθεια χρηστών σε εφαρμογές SaaS τρίτων κατασκευαστών, όπως το Salesforce, το G Suite και άλλα.</span><span class="sxs-lookup"><span data-stu-id="6f884-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="6f884-105">Εάν ενεργοποιήσετε την παροχή χρήστη για μια εφαρμογή SaaS άλλου κατασκευαστή, η πύλη Azure ελέγχει τις τιμές των χαρακτηριστικών του μέσω αντιστοιχίσεων χαρακτηριστικών.</span><span class="sxs-lookup"><span data-stu-id="6f884-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="6f884-106">Για να μάθετε πώς μπορείτε να προσαρμόσετε το προεπιλεγμένο χαρακτηριστικό-αντιστοιχίσεις, ανατρέξτε στο θέμα [Προσαρμογή χαρακτηριστικού παροχής χρήστη-αντιστοιχίσεις για εφαρμογές SaaS στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="6f884-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="6f884-107">Για να μάθετε περισσότερα σχετικά με την προμήθεια εφαρμογών SaaS, ανατρέξτε [στο θέμα Τι είναι η αυτοματοποιημένη προμήθεια εφαρμογών SaaS για χρήστες στο Azure AD;](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="6f884-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="6f884-108">Κατά την προσαρμογή των αντιστοιχίσεων χαρακτηριστικών για την προμήθεια του χρήστη, μπορεί να διαπιστώσετε ότι το χαρακτηριστικό που θέλετε να αντιστοιχίσετε δεν εμφανίζεται στη λίστα χαρακτηριστικών προέλευσης.</span><span class="sxs-lookup"><span data-stu-id="6f884-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="6f884-109">Ο [Συγχρονισμός ενός χαρακτηριστικού από την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης στο Azure AD για προμήθεια σε ένα](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) άρθρο της εφαρμογής σάς δείχνει πώς μπορείτε να προσθέσετε το χαρακτηριστικό που λείπει, πραγματοποιώντας συγχρονισμό του από τη διαφήμισή σας εσωτερικής εγκατάστασης στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f884-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
