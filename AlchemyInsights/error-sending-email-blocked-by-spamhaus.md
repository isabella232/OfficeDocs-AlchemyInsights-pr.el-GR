---
title: Σφάλμα κατά την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου αποκλεισμένο από το SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714258"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="736b1-102">Σφάλμα κατά την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου: Ο κεντρικός υπολογιστής πελάτη αποκλείστηκε με χρήση του Spamhaus</span><span class="sxs-lookup"><span data-stu-id="736b1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="736b1-103">Η διεύθυνση IP που έστειλε το μήνυμα βρίσκεται σε μια λίστα μπλοκ που ανήκει [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="736b1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="736b1-104">Οι λόγοι για τους οποίους μπλοκαρίστηκε από το Spamhaus περιλαμβάνουν λογαριασμούς που έχουν παραβιαστεί, υπολογιστές που έχουν παραβιαστεί και πολιτικές παροχής internet service (ISP).</span><span class="sxs-lookup"><span data-stu-id="736b1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="736b1-105">Πιθανές διορθώσεις είναι οι:</span><span class="sxs-lookup"><span data-stu-id="736b1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="736b1-106">Για αποκλεισμένα εισερχόμενα μηνύματα όπου ελέγχετε το διακομιστή ηλεκτρονικού ταχυδρομείου προέλευσης, πρέπει να προσδιορίσετε την αιτία και να καταργήσετε το μπλοκ από την τοποθεσία Web του Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="736b1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="736b1-107">Για αποκλεισμένα εισερχόμενα μηνύματα όπου η διεύθυνση IP προέλευσης ανήκει σε κάποιον άλλο, ο κάτοχος της διεύθυνσης πρέπει να καταργήσει το μπλοκ από την τοποθεσία Web του Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="736b1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="736b1-108">Εάν η διεύθυνση IP βρίσκεται στη λίστα μπλοκ πολιτικής (PBL), ο κάτοχος μπορεί να εκχωρήσει μια διαφορετική στατική διεύθυνση IP ή να καταργήσει τη διεύθυνση από το PBL.</span><span class="sxs-lookup"><span data-stu-id="736b1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="736b1-109">Για αποκλεισμένα εξερχόμενα μηνύματα από τον τομέα σας που είναι συνδεδεμένα με τη Microsoft, μπορείτε να λάβετε αυτό το σφάλμα, εάν τα μηνύματα δρομολογούνται μέσω μιας υπηρεσίας τρίτου κατασκευαστή.</span><span class="sxs-lookup"><span data-stu-id="736b1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="736b1-110">Μπορείτε να χρησιμοποιήσετε ένα εργαλείο αναζητήσεων WHOIS για να βρείτε τον αποκλεισμένο κάτοχο διεύθυνσης IP.</span><span class="sxs-lookup"><span data-stu-id="736b1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
