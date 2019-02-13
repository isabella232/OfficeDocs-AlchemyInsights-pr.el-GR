---
title: Σφάλμα κατά την αποστολή μηνύματος ηλεκτρονικού ταχυδρομείου που αποκλείονται από το SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912348"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="9944e-102">Σφάλμα κατά την αποστολή μηνύματος ηλεκτρονικού ταχυδρομείου: κεντρικός υπολογιστής-πελάτης αποκλειστούν χρησιμοποιώντας Spamhaus</span><span class="sxs-lookup"><span data-stu-id="9944e-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="9944e-p101">Η διεύθυνση IP που έστειλε το μήνυμα βρίσκεται σε μια λίστα αποκλεισμού που ανήκουν σε [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Λόγοι για να αποκλειστεί από Spamhaus περιλαμβάνουν λογαριασμούς έχει παραβιαστεί, διακυβεύεται μηχανές κοινή χρήση μιας δημόσιας διεύθυνσης IP και πολιτικές υπηρεσία παροχής Internet (ISP). Πιθανές ενημερώσεις κώδικα είναι οι εξής:</span><span class="sxs-lookup"><span data-stu-id="9944e-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="9944e-106">Για αποκλεισμένο εισερχόμενων μηνυμάτων στο Office 365, όπου μπορείτε να ελέγξετε το διακομιστή ηλεκτρονικού ταχυδρομείου προέλευσης, πρέπει να προσδιορίσετε την αιτία και να καταργήσετε τον αποκλεισμό από την τοποθεσία Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="9944e-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="9944e-p102">Για αποκλεισμένο εισερχόμενων μηνυμάτων στο Office 365, όπου η διεύθυνση προέλευσης IP ανήκει σε κάποιον άλλον, ο κάτοχος της διεύθυνσης πρέπει να καταργήσετε τον αποκλεισμό από την τοποθεσία Web Spamhaus. Εάν η διεύθυνση IP είναι στη λίστα αποκλεισμού πολιτικής (PBL), ο κάτοχος μπορεί να εκχωρήσετε διαφορετική στατική διεύθυνση IP ή να καταργήσετε τη διεύθυνση από το PBL.</span><span class="sxs-lookup"><span data-stu-id="9944e-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="9944e-p103">Για αποκλεισμένο εξερχόμενων μηνυμάτων από τον τομέα του Office 365, μπορείτε να λάβετε αυτό το σφάλμα, αν τα μηνύματα θα δρομολογούνται μέσω μιας υπηρεσίας τρίτου κατασκευαστή. Μπορείτε να χρησιμοποιήσετε ένα εργαλείο αναζήτησης WHOIS για να βρείτε κάτοχος αποκλεισμένη διεύθυνση IP.</span><span class="sxs-lookup"><span data-stu-id="9944e-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

