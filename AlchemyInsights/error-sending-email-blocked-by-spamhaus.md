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
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527133"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="2f433-102">Σφάλμα κατά την αποστολή μηνύματος ηλεκτρονικού ταχυδρομείου: κεντρικός υπολογιστής-πελάτης αποκλειστούν χρησιμοποιώντας Spamhaus</span><span class="sxs-lookup"><span data-stu-id="2f433-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="2f433-103">Η διεύθυνση IP που έστειλε το μήνυμα βρίσκεται σε μια λίστα αποκλεισμού που ανήκουν σε [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="2f433-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="2f433-104">Λόγοι για να αποκλειστεί από Spamhaus περιλαμβάνουν λογαριασμούς έχει παραβιαστεί, διακυβεύεται μηχανές κοινή χρήση μιας δημόσιας διεύθυνσης IP και πολιτικές υπηρεσία παροχής Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="2f433-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="2f433-105">Πιθανές ενημερώσεις κώδικα είναι οι εξής:</span><span class="sxs-lookup"><span data-stu-id="2f433-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="2f433-106">Για αποκλεισμένο εισερχόμενων μηνυμάτων στο Office 365, όπου μπορείτε να ελέγξετε το διακομιστή ηλεκτρονικού ταχυδρομείου προέλευσης, πρέπει να προσδιορίσετε την αιτία και να καταργήσετε τον αποκλεισμό από την τοποθεσία Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="2f433-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="2f433-107">Για αποκλεισμένο εισερχόμενων μηνυμάτων στο Office 365, όπου η διεύθυνση προέλευσης IP ανήκει σε κάποιον άλλον, ο κάτοχος της διεύθυνσης πρέπει να καταργήσετε τον αποκλεισμό από την τοποθεσία Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="2f433-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="2f433-108">Εάν η διεύθυνση IP είναι στη λίστα αποκλεισμού πολιτικής (PBL), ο κάτοχος μπορεί να εκχωρήσετε διαφορετική στατική διεύθυνση IP ή να καταργήσετε τη διεύθυνση από το PBL.</span><span class="sxs-lookup"><span data-stu-id="2f433-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="2f433-109">Για αποκλεισμένο εξερχόμενων μηνυμάτων από τον τομέα του Office 365, μπορείτε να λάβετε αυτό το σφάλμα, αν τα μηνύματα θα δρομολογούνται μέσω μιας υπηρεσίας τρίτου κατασκευαστή.</span><span class="sxs-lookup"><span data-stu-id="2f433-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="2f433-110">Μπορείτε να χρησιμοποιήσετε ένα εργαλείο αναζήτησης WHOIS για να βρείτε κάτοχος αποκλεισμένη διεύθυνση IP.</span><span class="sxs-lookup"><span data-stu-id="2f433-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
