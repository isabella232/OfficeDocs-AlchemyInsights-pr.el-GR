---
title: Σφάλμα ομάδων 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796136"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="c9299-102">σφάλμα 4c7 στις ομάδες της Microsoft</span><span class="sxs-lookup"><span data-stu-id="c9299-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="c9299-103">Αυτό το σφάλμα παρουσιάζεται επειδή οι ομάδες της Microsoft απαιτεί έλεγχο ταυτότητας φορμών.</span><span class="sxs-lookup"><span data-stu-id="c9299-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="c9299-104">Όταν αναπτύσσετε υπηρεσίες Ομοσπονδία Active Directory (AD ΛΕ), έλεγχος ταυτότητας φορμών δεν είναι ενεργοποιημένη για το intranet από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="c9299-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="c9299-105">Εάν αποτύχει ο ενσωματωμένος έλεγχος ταυτότητας των Windows, θα σας ζητηθεί να εισέλθετε χρησιμοποιώντας τον έλεγχο ταυτότητας φορμών.</span><span class="sxs-lookup"><span data-stu-id="c9299-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="c9299-106">Για να επιλύσετε αυτό το ζήτημα, ενεργοποιήστε τον έλεγχο ταυτότητας φορμών, χρησιμοποιώντας το συμπληρωματικό πρόγραμμα AD FS κονσόλας διαχείρισης της Microsoft (MMC) στον υπολογιστή που διαθέτει το τοπικό αντίγραφο της υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c9299-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="c9299-107">Για να το κάνετε, ακολουθήστε αυτά τα βήματα:</span><span class="sxs-lookup"><span data-stu-id="c9299-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="c9299-108">Στο παράθυρο περιήγησης, αναζητήστε τις **πολιτικές ελέγχου ταυτότητας**.</span><span class="sxs-lookup"><span data-stu-id="c9299-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="c9299-109">Στην περιοχή **ενέργειες** στο παράθυρο λεπτομερειών, επιλέξτε **Επεξεργασία καθολικού πρωτεύοντος ελέγχου ταυτότητας**.</span><span class="sxs-lookup"><span data-stu-id="c9299-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="c9299-110">Στην καρτέλα **intranet** , επιλέξτε **Έλεγχος ταυτότητας φορμών**.</span><span class="sxs-lookup"><span data-stu-id="c9299-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="c9299-111">Επιλέξτε **OK** (ή **Εφαρμόστε**).</span><span class="sxs-lookup"><span data-stu-id="c9299-111">Select **OK** (or **Apply**).</span></span>