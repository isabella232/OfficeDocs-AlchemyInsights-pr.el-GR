---
title: Προσομοιωτής επίθεσης του 2681 στο Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801551"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="4d7e3-102">Προσομοιωτής επίθεσης στο Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4d7e3-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="4d7e3-103">Σας λείπει ο προσομοιωτής επίθεσης;</span><span class="sxs-lookup"><span data-stu-id="4d7e3-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="4d7e3-104">Ο προσομοιωτής επίθεσης απαιτεί **από το Microsoft Defender για το office 365 πρόγραμμα 2 (ATP Plan 2) ή το** **Office 365 για μεγάλες επιχειρήσεις E5** .</span><span class="sxs-lookup"><span data-stu-id="4d7e3-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="4d7e3-105">Ο προσομοιωτής επίθεσης **δεν** περιλαμβάνεται στο Microsoft Defender για το Office 365 Plan 1 (ATP Plan 1), το Office 365 Enterprise E3 ή οποιαδήποτε εφαρμογή εφαρμογών Microsoft 365 για επιχειρηματικές συνδρομές.</span><span class="sxs-lookup"><span data-stu-id="4d7e3-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="4d7e3-106">Ο λογαριασμός που χρησιμοποιείτε για την εκκίνηση προσομοιωμένων επιθέσεων απαιτεί καθολικό διαχειριστή ή δικαιώματα διαχειριστή ασφαλείας και έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ).</span><span class="sxs-lookup"><span data-stu-id="4d7e3-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="4d7e3-107">Για περισσότερες πληροφορίες σχετικά με τις απαιτήσεις του προσομοιωτή επίθεσης, ανατρέξτε σε [αυτό το θέμα](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="4d7e3-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="4d7e3-108">Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με τις προσομοιώσεις επίθεσης με **κωδικό πρόσβασης ωμής βίας** :</span><span class="sxs-lookup"><span data-stu-id="4d7e3-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="4d7e3-109">Εάν ο λογαριασμός προορισμού έχει ενεργοποιημένη τη λειτουργία ΣΠΙ και ο κωδικός πρόσβασης έχει υποτεθεί σωστά, ο λογαριασμός δεν θα εμφανίζεται ως εκτεθειμένος (ο δεύτερος παράγοντας ελέγχου ταυτότητας θα είναι ελλιπής).</span><span class="sxs-lookup"><span data-stu-id="4d7e3-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="4d7e3-110">Το αρχείο κωδικού πρόσβασης δεν μπορεί να είναι μεγαλύτερο από 10 MB.</span><span class="sxs-lookup"><span data-stu-id="4d7e3-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="4d7e3-111">Χρησιμοποιήστε έναν κωδικό πρόσβασης ανά γραμμή και συμπεριλάβετε μια κενή γραμμή (επιστροφή) μετά τον τελευταίο κωδικό πρόσβασης στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="4d7e3-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="4d7e3-112">Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με το **δόρυ phishing** επισυνάψτε προσομοιώσεις:</span><span class="sxs-lookup"><span data-stu-id="4d7e3-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="4d7e3-113">Κατά τη σχεδίαση, δεν μπορείτε να παρέχετε μια προσαρμοσμένη τιμή για τη **διεύθυνση URL του διακομιστή σύνδεσης ηλεκτρονικού "ψαρέματος"** .</span><span class="sxs-lookup"><span data-stu-id="4d7e3-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="4d7e3-114">Εάν ένας παραλήπτης χρησιμοποιήσει την [Ενεργοποίηση του πρόσθετου μηνύματος αναφοράς](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) για να αναφέρει το μήνυμα ως ηλεκτρονικό "ψάρεμα", ενδέχεται να μην λαμβάνετε ειδοποιήσεις για το μήνυμα (επειδή πρόκειται για προσομοίωση επίθεσης).</span><span class="sxs-lookup"><span data-stu-id="4d7e3-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="4d7e3-115">Αναφορές: μετά την ολοκλήρωση της προσομοιωμένης επίθεσης, μπορείτε να κάνετε κλικ στην επιλογή **Λεπτομέρειες επίθεσης** για να δείτε την αναφορά.</span><span class="sxs-lookup"><span data-stu-id="4d7e3-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="4d7e3-116">Για λεπτομερείς οδηγίες και νέες δυνατότητες στον προσομοιωτή επίθεσης, ανατρέξτε [στο θέμα προσομοιωτής επίθεσης στο Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="4d7e3-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
