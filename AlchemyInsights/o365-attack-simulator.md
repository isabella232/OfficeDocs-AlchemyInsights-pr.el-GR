---
title: 2681 Attack Simulator στο Microsoft 365
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545726"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="42b95-102">Ο Εξομοιωτής επίθεσης Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="42b95-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="42b95-103">Σας λείπει ο Εξομοιωτής επίθεσης;</span><span class="sxs-lookup"><span data-stu-id="42b95-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="42b95-104">Το Attack Defender **απαιτεί τον Microsoft Defender Office 365 πρόγραμμα 2** ή Office 365 για μεγάλες επιχειρήσεις **E5.**</span><span class="sxs-lookup"><span data-stu-id="42b95-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="42b95-105">Το Attack Simulator **δεν** περιλαμβάνεται στο Microsoft Defender για Office 365 Πρόγραμμα 1, Office 365 για μεγάλες επιχειρήσεις E3 ή σε Εφαρμογές Microsoft 365 για επιχειρήσεις συνδρομές.</span><span class="sxs-lookup"><span data-stu-id="42b95-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="42b95-106">Ο λογαριασμός που χρησιμοποιείτε για την εκκίνηση προσομοιωμενών επιθέσεων απαιτεί δικαιώματα καθολικού διαχειριστή ή διαχειριστή ασφαλείας και έλεγχο ταυτότητας πολλών παραγόντων (MFA).</span><span class="sxs-lookup"><span data-stu-id="42b95-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="42b95-107">Για περισσότερες πληροφορίες σχετικά με τις απαιτήσεις του Attack Simulator, ανατρέξτε [σε αυτό το θέμα.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="42b95-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="42b95-108">Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με τις **προσομοιώσεις επίθεσης του Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="42b95-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="42b95-109">Εάν ο λογαριασμός προορισμού έχει ενεργοποιήσει το MFA και ο κωδικός πρόσβασης έχει γίνει σωστή μαντέψει, ο λογαριασμός δεν θα εμφανίζεται ως παραβιαστείς (ο δεύτερος παράγοντας ελέγχου ταυτότητας θα είναι ημιτελής).</span><span class="sxs-lookup"><span data-stu-id="42b95-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="42b95-110">Το αρχείο κωδικού πρόσβασης δεν μπορεί να είναι μεγαλύτερο από 10 MB.</span><span class="sxs-lookup"><span data-stu-id="42b95-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="42b95-111">Χρησιμοποιήστε έναν κωδικό πρόσβασης ανά γραμμή και συμπεριλάβετε μια κενή γραμμή (επαναφορά) μετά τον τελευταίο κωδικό πρόσβασης στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="42b95-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="42b95-112">Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με την **επισύναψη προσομοιώσεων ηλεκτρονικού "ψαρέματος** με δόρυ":</span><span class="sxs-lookup"><span data-stu-id="42b95-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="42b95-113">Από τη σχεδίαση, δεν μπορείτε να δώσετε μια προσαρμοσμένη τιμή για τη διεύθυνση URL του διακομιστή **σύνδεσης ηλεκτρονικού "ψαρέματος".**</span><span class="sxs-lookup"><span data-stu-id="42b95-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="42b95-114">Εάν ένας παραλήπτης χρησιμοποιεί το πρόσθετο ["Ενεργοποίηση](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) μηνύματος αναφοράς" για να αναφέρει το μήνυμα ως ηλεκτρονικό "ψάρεμα", ενδέχεται να μην λαμβάνετε ειδοποιήσεις για το μήνυμα (επειδή πρόκειται για προσομοιωμένη επίθεση).</span><span class="sxs-lookup"><span data-stu-id="42b95-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="42b95-115">Αναφορές: Μετά την ολοκλήρωση της προσομοιωμένης επίθεσης, μπορείτε να κάνετε κλικ **στην επιλογή "Λεπτομέρειες επίθεσης"** για να δείτε την αναφορά.</span><span class="sxs-lookup"><span data-stu-id="42b95-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="42b95-116">Για λεπτομερείς οδηγίες και νέες δυνατότητες στον Εξομοιωτή επίθεσης, ανατρέξτε στο θέμα ["Προσομοίωση επίθεσης" Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="42b95-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
