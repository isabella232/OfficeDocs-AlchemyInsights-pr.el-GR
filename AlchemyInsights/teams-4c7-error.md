---
title: Σφάλμα 4c7 ομάδων
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700203"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="ddc4e-102">σφάλμα 4c7 στο Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="ddc4e-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="ddc4e-103">Αυτό το σφάλμα παρουσιάζεται επειδή το Microsoft teams απαιτεί έλεγχο ταυτότητας φορμών.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="ddc4e-104">Κατά την ανάπτυξη των υπηρεσιών Ομοσπονδία υπηρεσίας καταλόγου Active Directory (AD FS), ο έλεγχος ταυτότητας φορμών δεν είναι ενεργοποιημένος για το intranet από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="ddc4e-105">Εάν αποτύχει ο ενσωματωμένος έλεγχος ταυτότητας των Windows, θα σας ζητηθεί να πραγματοποιήσετε είσοδο χρησιμοποιώντας τον έλεγχο ταυτότητας φορμών.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="ddc4e-106">Για να επιλύσετε αυτό το ζήτημα, ενεργοποιήστε τον έλεγχο ταυτότητας φορμών χρησιμοποιώντας το συμπληρωματικό πρόγραμμα της κονσόλας διαχείρισης της Microsoft (MMC) AD FS στον υπολογιστή που έχει το τοπικό αντίγραφο της υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="ddc4e-107">Για να το κάνετε, ακολουθήστε αυτά τα βήματα:</span><span class="sxs-lookup"><span data-stu-id="ddc4e-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="ddc4e-108">Στο παράθυρο περιήγησης, μεταβείτε στις **πολιτικές ελέγχου ταυτότητας**.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="ddc4e-109">Στην περιοχή **ενέργειες** στο παράθυρο λεπτομερειών, επιλέξτε **Επεξεργασία καθολικού πρωτεύοντος ελέγχου ταυτότητας**.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="ddc4e-110">Στην καρτέλα **intranet** , επιλέξτε **Έλεγχος ταυτότητας φορμών**.</span><span class="sxs-lookup"><span data-stu-id="ddc4e-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="ddc4e-111">Επιλέξτε **OK** (ή **Apply**).</span><span class="sxs-lookup"><span data-stu-id="ddc4e-111">Select **OK** (or **Apply**).</span></span>