---
title: Ανάπτυξη GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427254"
---
# <a name="gpo-deployment"></a><span data-ttu-id="96109-102">Ανάπτυξη GPO</span><span class="sxs-lookup"><span data-stu-id="96109-102">GPO Deployment</span></span>

<span data-ttu-id="96109-103">Η διαχείριση των ρυθμίσεων για αντικείμενα χρηστών και υπολογιστών στις υπηρεσίες τομέα Azure Active Directory (Azure AD DS) γίνεται συχνά με τη χρήση αντικειμένων πολιτικής ομάδας (GPOs).</span><span class="sxs-lookup"><span data-stu-id="96109-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="96109-104">Το Azure AD DS περιλαμβάνει ενσωματωμένα GPOs για τους χρήστες AADDC και τα κοντέινερ υπολογιστών AADDC.</span><span class="sxs-lookup"><span data-stu-id="96109-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="96109-105">Μπορείτε να προσαρμόσετε αυτά τα ενσωματωμένα GPOs για να ρυθμίσετε τις παραμέτρους της πολιτικής ομάδας ανάλογα με τις ανάγκες για το περιβάλλον σας.</span><span class="sxs-lookup"><span data-stu-id="96109-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="96109-106">Τα μέλη της ομάδας διαχειριστών DC του Azure AD έχουν δικαιώματα διαχείρισης πολιτικής ομάδας στον τομέα Azure AD DS και μπορούν επίσης να δημιουργήσουν προσαρμοσμένα GPOs και εταιρικές μονάδες (OUs).</span><span class="sxs-lookup"><span data-stu-id="96109-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="96109-107">Για περισσότερες πληροφορίες σχετικά με την πολιτική ομάδας και τον τρόπο που λειτουργεί, ανατρέξτε στο θέμα ["Επισκόπηση πολιτικής ομάδας".](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="96109-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="96109-108">Σε ένα υβριδικό περιβάλλον, οι πολιτικές ομάδας που έχουν ρυθμιστεί σε περιβάλλον AD DS εσωτερικής εγκατάστασης δεν συγχρονίζονται με το Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="96109-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="96109-109">Για να ορίσετε ρυθμίσεις παραμέτρων για χρήστες ή υπολογιστές στο Azure AD DS, επεξεργαστείτε ένα από τα προεπιλεγμένα GPOs ή δημιουργήστε ένα προσαρμοσμένο GPO.</span><span class="sxs-lookup"><span data-stu-id="96109-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="96109-110">Αυτό το [άρθρο "Διαχείριση](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) πολιτικής ομάδας" σάς δείχνει πώς μπορείτε να εγκαταστήσετε τα εργαλεία διαχείρισης πολιτικής ομάδας, πώς μπορείτε να επεξεργαστείτε τα ενσωματωμένα GPOs και πώς μπορείτε να δημιουργήσετε προσαρμοσμένα GPOs.</span><span class="sxs-lookup"><span data-stu-id="96109-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
