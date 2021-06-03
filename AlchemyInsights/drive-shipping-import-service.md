---
title: Αποστολή μονάδας δίσκου στην υπηρεσία Microsoft 365 εισαγωγής
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731648"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="7b1ba-102">Αποστολή μονάδας δίσκου στην υπηρεσία Microsoft 365 εισαγωγής</span><span class="sxs-lookup"><span data-stu-id="7b1ba-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="7b1ba-103">Χρησιμοποιήστε την αποστολή μονάδας δίσκου αντιγράφοντας psTs σε έναν σκληρό δίσκο και, στη συνέχεια, στέλνοντας τον σκληρό δίσκο στη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="7b1ba-104">Για να ξεκινήσετε την εργασία:</span><span class="sxs-lookup"><span data-stu-id="7b1ba-104">To start the job:</span></span>

1. <span data-ttu-id="7b1ba-105">Στο κέντρο Microsoft 365 συμμόρφωσης στην περιοχή **"Διαχείριση πληροφοριών",** επιλέξτε **"Εισαγωγή".**</span><span class="sxs-lookup"><span data-stu-id="7b1ba-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="7b1ba-106">Επιλέξτε **"Επιλογή τύπου εργασίας εισαγωγής" και,** στη συνέχεια, επιλέξτε **"Επόμενο".**</span><span class="sxs-lookup"><span data-stu-id="7b1ba-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="7b1ba-107">Για να δείτε τα βήματα για αυτή την επιλογή εισαγωγής, επιλέξτε **"Αποστολή σκληρών δίσκων" σε μία από τις φυσικές θέσεις μας.**</span><span class="sxs-lookup"><span data-stu-id="7b1ba-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="7b1ba-108">Ακολουθούν ορισμένα πράγματα που πρέπει να θυμάστε:</span><span class="sxs-lookup"><span data-stu-id="7b1ba-108">Here are some things to remember:</span></span>

- <span data-ttu-id="7b1ba-109">Πρέπει να σας εκχωρηθεί ο ρόλος "Εξαγωγή εισαγωγής γραμματοκιβωτίου" Exchange Online να εισαγάγετε αρχεία PST σε Microsoft 365 γραμματοκιβώτια.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="7b1ba-110">Οι επιδόσεις ενδέχεται να επηρεάσουν τις PSTs μεγαλύτερες από 20 GB.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="7b1ba-111">Υποστηρίζονται μόνο μονάδες σκληρού δίσκου σταθερής κατάστασης 2,5 ιντσών (SSDs) ή 2,5 ιντσών ή 3,5 ιντσών SATA II/III.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="7b1ba-112">Ο σκληρός δίσκος που περιέχει αρχεία PST πρέπει να είναι κρυπτογραφημένος με BitLocker.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="7b1ba-113">Το κόστος για την εισαγωγή αρχείων PST Microsoft 365 γραμματοκιβώτια χρησιμοποιώντας την αποστολή μονάδας δίσκου είναι 2 δολάρια ΗΠΑ ανά GB δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="7b1ba-114">Για πρόσθετες πληροφορίες σχετικά με τη χρήση της μεθόδου αποστολής μονάδας δίσκου για την εισαγωγή PSTs, ανατρέξτε στο θέμα Χρήση αποστολής μονάδας δίσκου για [την εισαγωγή αρχείων PST του οργανισμού σας.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="7b1ba-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>