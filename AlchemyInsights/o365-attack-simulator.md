---
title: 2681 προσομοιωτή επίθεση στο γραφείο 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305332"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="5ca02-102">Προσομοιωτή επίθεση στο γραφείο 365</span><span class="sxs-lookup"><span data-stu-id="5ca02-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="5ca02-103">Σου λείπει ο προσομοιωτής επίθεσης;</span><span class="sxs-lookup"><span data-stu-id="5ca02-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="5ca02-104">Επίθεση προσομοιωτή απαιτεί **office 365 προηγμένη προστασία απειλή σχέδιο 2 (ATP σχέδιο 2)** ή **Office 365 Enterprise**Ε2.</span><span class="sxs-lookup"><span data-stu-id="5ca02-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="5ca02-105">Επίθεση προσομοιωτή **δεν** περιλαμβάνεται στο Office 365 σύνθετη προστασία απειλή σχέδιο 1 (ATP σχέδιο 1), Office 365 Enterprise ε ή οποιεσδήποτε συνδρομές Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="5ca02-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="5ca02-106">Ο λογαριασμός που χρησιμοποιείτε για την εκκίνηση προσομοιωμένων επιθέσεων απαιτεί καθολικά δικαιώματα διαχειριστή ή διαχειριστή ασφαλείας και έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ).</span><span class="sxs-lookup"><span data-stu-id="5ca02-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="5ca02-107">Για περισσότερες πληροφορίες σχετικά με τις απαιτήσεις επίθεσης Simulator, ανατρέξτε σε [αυτό το θέμα](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="5ca02-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="5ca02-108">Σημαντικά πράγματα που πρέπει να γνωρίζετε για τις προσομοιώσεις επίθεσης με **κωδικό πρόσβασης σε ωμή δύναμη** :</span><span class="sxs-lookup"><span data-stu-id="5ca02-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="5ca02-109">Εάν ο λογαριασμός στόχου έχει ΜΧΣ ενεργοποιημένη και ο κωδικός πρόσβασης έχει μαντέψει σωστά, ο λογαριασμός δεν θα εμφανιστεί σε κίνδυνο (ο δεύτερος συντελεστής ελέγχου ταυτότητας θα είναι ελλιπής).</span><span class="sxs-lookup"><span data-stu-id="5ca02-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="5ca02-110">Το αρχείο κωδικού πρόσβασης δεν μπορεί να είναι μεγαλύτερο από 10 MB.</span><span class="sxs-lookup"><span data-stu-id="5ca02-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="5ca02-111">Χρησιμοποιήστε έναν κωδικό πρόσβασης ανά γραμμή και συμπεριλάβετε μια κενή γραμμή (επιστροφή επαναφοράς) μετά τον τελευταίο κωδικό πρόσβασης στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="5ca02-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="5ca02-112">Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με το **δόρυ phishing** επισυνάπτει προσομοιώσεις:</span><span class="sxs-lookup"><span data-stu-id="5ca02-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="5ca02-113">Κατά τη σχεδίαση, δεν μπορείτε να παρέχετε μια προσαρμοσμένη τιμή για τη **διεύθυνση URL του διακομιστή σύνδεσης phishing**.</span><span class="sxs-lookup"><span data-stu-id="5ca02-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="5ca02-114">Εάν ένας παραλήπτης χρησιμοποιεί το [πρόσθετο "Ενεργοποίηση του μηνύματος αναφοράς](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " για να αναφέρει το μήνυμα ως ηλεκτρονικό ψάρεμα, ενδέχεται να μην λαμβάνετε ειδοποιήσεις για το μήνυμα (επειδή πρόκειται για προσομοίωση επίθεσης).</span><span class="sxs-lookup"><span data-stu-id="5ca02-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="5ca02-115">Αναφορές: μετά την ολοκλήρωση της προσομοίωσης επίθεσης, μπορείτε να κάνετε κλικ στην επιλογή **Λεπτομέρειες επίθεσης** για να δείτε την αναφορά.</span><span class="sxs-lookup"><span data-stu-id="5ca02-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="5ca02-116">Για αναλυτικές οδηγίες και νέες δυνατότητες στο επίθεση Simulator, ανατρέξτε [στο τμήμα προσομοίωσης επίθεσης στο Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="5ca02-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
