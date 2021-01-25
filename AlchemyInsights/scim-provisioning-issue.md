---
title: Θέμα προμήθειας SCIM
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949786"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="05ec6-102">Θέμα προμήθειας SCIM</span><span class="sxs-lookup"><span data-stu-id="05ec6-102">SCIM provisioning issue</span></span>

<span data-ttu-id="05ec6-103">Η αυτόματη προμήθεια αναφέρεται στη δημιουργία ταυτοτήτων χρηστών και ρόλων στις εφαρμογές cloud στις οποίες οι χρήστες χρειάζονται πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="05ec6-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="05ec6-104">Εκτός από τη δημιουργία ταυτοτήτων χρηστών, η αυτόματη προμήθεια περιλαμβάνει τη συντήρηση και την κατάργηση των ταυτοτήτων χρηστών ως αλλαγή κατάστασης ή ρόλων.</span><span class="sxs-lookup"><span data-stu-id="05ec6-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="05ec6-105">Πριν ξεκινήσετε μια ανάπτυξη, μπορείτε να δείτε [Πώς λειτουργεί](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) η προμήθεια για να μάθετε τον τρόπο με τον οποίο λειτουργεί η παροχή Azure Active Directory (AD) και να λάβετε προτάσεις ρύθμισης παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="05ec6-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="05ec6-106">Ως προγραμματιστής εφαρμογών, μπορείτε να χρησιμοποιήσετε το API διαχείρισης διαχείρισης ταυτοτήτων μεταξύ τομέων (SCIM) για να ενεργοποιήσετε την αυτόματη προμήθεια χρηστών και ομάδων μεταξύ της εφαρμογής σας και του Azure AD.</span><span class="sxs-lookup"><span data-stu-id="05ec6-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="05ec6-107">Το [τελικό σημείο δόμησης SCIM και η ρύθμιση παραμέτρων παροχής χρήστη με το άρθρο AD Azure](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) περιγράφει τον τρόπο δημιουργίας ενός τελικού σημείου SCIM και την ενσωμάτωσή του με την υπηρεσία ΠΑΡΟΧΉς Azure AD.</span><span class="sxs-lookup"><span data-stu-id="05ec6-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



