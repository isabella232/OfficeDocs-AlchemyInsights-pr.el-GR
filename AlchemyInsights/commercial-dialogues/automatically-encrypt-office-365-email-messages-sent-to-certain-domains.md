---
title: Αυτόματη κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου του Office 365 που αποστέλλονται σε ορισμένους τομείς
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746052"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="f63f8-102">Αυτόματη κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου του Office 365 που αποστέλλονται σε ορισμένους τομείς</span><span class="sxs-lookup"><span data-stu-id="f63f8-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="f63f8-103">Από το [κέντρο διαχείρισης του Exchange,](https://outlook.office365.com/ecp/)επιλέξτε **κανόνες ροής > αλληλογραφίας.**</span><span class="sxs-lookup"><span data-stu-id="f63f8-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="f63f8-104">Κάντε κλικ στο **εικονίδιο "Δημιουργία" (+)** και, στη συνέχεια, κάντε κλικ στην επιλογή "Εφαρμογή κρυπτογράφησης μηνυμάτων του **Office 365" και προστασία δικαιωμάτων σε μηνύματα.**</span><span class="sxs-lookup"><span data-stu-id="f63f8-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="f63f8-105">Στο **πεδίο "Όνομα",** πληκτρολογήστε ένα όνομα για τον κανόνα, όπως "Κρυπτογράφηση μηνυμάτων που αποστέλλονται σε *contoso.com".*</span><span class="sxs-lookup"><span data-stu-id="f63f8-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="f63f8-106">Στην **περιοχή "Εφαρμογή αυτού του κανόνα",** εάν , **επιλέξτε "Ο παραλήπτης > τομέα" είναι**.</span><span class="sxs-lookup"><span data-stu-id="f63f8-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="f63f8-107">Πληκτρολογήστε το όνομα του τομέα, όπως **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="f63f8-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="f63f8-108">Κάντε κλικ στο **εικονίδιο Προσθήκη (+) και,** στη συνέχεια, κάντε κλικ στο **κουμπί OK.**</span><span class="sxs-lookup"><span data-stu-id="f63f8-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="f63f8-109">Δίπλα στο πεδίο **"Να γίνει το εξής",** κάντε κλικ **στην επιλογή "Επιλογή ενός".**</span><span class="sxs-lookup"><span data-stu-id="f63f8-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="f63f8-110">Στο αναπτυσσόμενο **μενού προτύπου RMS,** επιλέξτε "Κρυπτογράφηση" **και,** στη συνέχεια, κάντε κλικ στο **κουμπί OK.**</span><span class="sxs-lookup"><span data-stu-id="f63f8-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="f63f8-111">(Εάν δεν βλέπετε αυτή την επιλογή, αυτό σημαίνει ότι το σχέδιό σας δεν περιλαμβάνει αυτόματη κρυπτογράφηση.</span><span class="sxs-lookup"><span data-stu-id="f63f8-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="f63f8-112">Ωστόσο, μπορείτε να το προσθέσετε!)</span><span class="sxs-lookup"><span data-stu-id="f63f8-112">But you can add it!)</span></span>
9. <span data-ttu-id="f63f8-113">Επιλέξτε οποιαδήποτε προαιρετική επιλογή (από μια λίστα προαιρετικών επιλογών που μπορείτε να κάνετε σε αυτό το σημείο, πολλές από τις οποίες μπορεί να τίθενται με την προεπιλεγμένη ρύθμιση για απλότητα).</span><span class="sxs-lookup"><span data-stu-id="f63f8-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="f63f8-114">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="f63f8-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f63f8-115">Μπορείτε πάντα να ξανάρθετε και να επεξεργαστείτε αυτόν τον κανόνα αργότερα.</span><span class="sxs-lookup"><span data-stu-id="f63f8-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="f63f8-116">Για περισσότερες πληροφορίες σχετικά με τη δημιουργία κανόνων κρυπτογράφησης, ανατρέξτε στο θέμα Ορισμός κανόνων ροής αλληλογραφίας για την κρυπτογράφηση μηνυμάτων [ηλεκτρονικού ταχυδρομείου στο Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="f63f8-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>