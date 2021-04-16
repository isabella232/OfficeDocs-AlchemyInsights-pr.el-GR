---
title: Σφάλμα κατά την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου που έχουν αποκλειστεί από την SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813724"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="c8f1c-102">Σφάλμα κατά την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου: Ο κεντρικός υπολογιστής-πελάτης αποκλείσθηκε χρησιμοποιώντας το Spamhaus</span><span class="sxs-lookup"><span data-stu-id="c8f1c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="c8f1c-103">Η διεύθυνση IP που έστειλε το μήνυμα βρίσκεται σε μια λίστα αποκλεισμού που ανήκει στην [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="c8f1c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="c8f1c-104">Οι λόγοι αποκλεισμού από την Spamhaus περιλαμβάνουν λογαριασμούς που έχουν παραβιαστεί, υπολογιστές που έχουν παραβιαστεί και μοιράζονται μια δημόσια διεύθυνση IP και πολιτικές υπηρεσίας παροχής Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="c8f1c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="c8f1c-105">Πιθανές επιδιορθώσεις είναι οι εξής:</span><span class="sxs-lookup"><span data-stu-id="c8f1c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="c8f1c-106">Για αποκλεισμένα εισερχόμενα μηνύματα όπου ελέγχετε το διακομιστή ηλεκτρονικού ταχυδρομείου προέλευσης, πρέπει να προσδιορίσετε την αιτία και να καταργήσετε το μπλοκ από την τοποθεσία Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="c8f1c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="c8f1c-107">Για αποκλεισμένα εισερχόμενα μηνύματα όπου η διεύθυνση IP προέλευσης ανήκει σε κάποιον άλλο, ο κάτοχος της διεύθυνσης πρέπει να καταργήσει το μπλοκ από την τοποθεσία Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="c8f1c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="c8f1c-108">Εάν η διεύθυνση IP βρίσκεται στη λίστα αποκλεισμού πολιτικής (PBL), ο κάτοχος μπορεί να αντιστοιχίσει μια διαφορετική στατική διεύθυνση IP ή να καταργήσει τη διεύθυνση από το PBL.</span><span class="sxs-lookup"><span data-stu-id="c8f1c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="c8f1c-109">Για αποκλεισμένα εξερχόμενα μηνύματα από τον τομέα σας που είναι συνδεδεμένα με τη Microsoft, μπορείτε να λάβετε αυτό το σφάλμα εάν τα μηνύματα δρομολογούνται μέσω μιας υπηρεσίας τρίτου κατασκευαστή.</span><span class="sxs-lookup"><span data-stu-id="c8f1c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="c8f1c-110">Μπορείτε να χρησιμοποιήσετε ένα εργαλείο αναζήτησης WHOIS για να βρείτε τον αποκλεισμένο κάτοχο διεύθυνσης IP.</span><span class="sxs-lookup"><span data-stu-id="c8f1c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
