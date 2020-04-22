---
title: 2681 Προσομοιωτής επίθεσης στο Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713466"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="72414-102">Προσομοιωτής επίθεσης στο Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="72414-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="72414-103">Σας λείπει ο προσομοιωτής επίθεσης;</span><span class="sxs-lookup"><span data-stu-id="72414-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="72414-104">Το Attack Simulator απαιτεί **το Πρόγραμμα προστασίας από απειλές για προχωρημένους του Office 365 (Σχέδιο ATP 2)** ή **το Office 365 για μεγάλες επιχειρήσεις E5**.</span><span class="sxs-lookup"><span data-stu-id="72414-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="72414-105">Το Attack Simulator **δεν** περιλαμβάνεται στο Πρόγραμμα προστασίας από απειλές για προχωρημένους του Office 365 (Πρόγραμμα ATP 1), στο Office 365 για μεγάλες επιχειρήσεις E3 ή σε οποιεσδήποτε συνδρομές microsoft 365 εφαρμογών για επιχειρήσεις.</span><span class="sxs-lookup"><span data-stu-id="72414-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="72414-106">Ο λογαριασμός που χρησιμοποιείτε για την έναρξη προσομοιωμένες επιθέσεις απαιτεί καθολικά δικαιώματα διαχειριστή ή διαχειριστή ασφαλείας και έλεγχο ταυτότητας πολλών παραγόντων (MFA).</span><span class="sxs-lookup"><span data-stu-id="72414-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="72414-107">Για περισσότερες πληροφορίες σχετικά με τις απαιτήσεις του Attack Simulator, ανατρέξτε [σε αυτό το θέμα](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="72414-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="72414-108">Σημαντικά πράγματα που πρέπει να ξέρετε για τις προσομοιώσεις **επίθεσης με κωδικό πρόσβασης ωμής βίας:**</span><span class="sxs-lookup"><span data-stu-id="72414-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="72414-109">Εάν ο λογαριασμός προορισμού έχει ενεργοποιημένη τη Δυνατότητα Υπα /να έχει ενεργοποιημένη τη Δυνατότητα Πρόσβασης και ο κωδικός πρόσβασης έχει μαντέψει σωστά, ο λογαριασμός δεν θα εμφανίζεται ως παραβιασμένος (ο δεύτερος παράγοντας ελέγχου ταυτότητας θα είναι ελλιπής).</span><span class="sxs-lookup"><span data-stu-id="72414-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="72414-110">Το αρχείο κωδικού πρόσβασης δεν μπορεί να είναι μεγαλύτερο από 10 MB.</span><span class="sxs-lookup"><span data-stu-id="72414-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="72414-111">Χρησιμοποιήστε έναν κωδικό πρόσβασης ανά γραμμή και συμπεριλάβετε μια κενή γραμμή (επαναφορά μεταφοράς) μετά τον τελευταίο κωδικό πρόσβασης στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="72414-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="72414-112">Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με το **Spear Phishing** επισυνάψτε προσομοιώσεις:</span><span class="sxs-lookup"><span data-stu-id="72414-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="72414-113">Κατά σχεδίαση, δεν μπορείτε να παρέχετε μια προσαρμοσμένη τιμή για **τη διεύθυνση URL του διακομιστή σύνδεσης ηλεκτρονικού "ψαρέματος"**.</span><span class="sxs-lookup"><span data-stu-id="72414-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="72414-114">Εάν ένας παραλήπτης χρησιμοποιεί [το πρόσθετο Ενεργοποίηση του μηνύματος αναφοράς](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) για να αναφέρει το μήνυμα ως ηλεκτρονικό ψάρεμα (phishing), ενδέχεται να μην λαμβάνετε ειδοποιήσεις για το μήνυμα (επειδή πρόκειται για προσομοιωμένη επίθεση).</span><span class="sxs-lookup"><span data-stu-id="72414-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="72414-115">Αναφορές: Μετά την ολοκλήρωση της προσομοιωμένης επίθεσης, μπορείτε να κάνετε κλικ στην επιλογή **Λεπτομέρειες επίθεσης** για να δείτε την αναφορά.</span><span class="sxs-lookup"><span data-stu-id="72414-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="72414-116">Για λεπτομερείς οδηγίες και νέες δυνατότητες στο Attack Simulator, ανατρέξτε στο θέμα [Προσομοιωτής επίθεσης στο Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="72414-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
