---
title: Υποβολή μηνύματος ηλεκτρονικού ταχυδρομείου παρέχοντας το αναγνωριστικό του μηνύματος δικτύου
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693918"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="2ca5f-102">Υποβολή μηνύματος ηλεκτρονικού ταχυδρομείου παρέχοντας το αναγνωριστικό του μηνύματος δικτύου</span><span class="sxs-lookup"><span data-stu-id="2ca5f-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="2ca5f-103">Στο αναδυόμενο **στοιχείο "Νέα υποβολή",** επιλέξτε **"Ηλεκτρονικό ταχυδρομείο"** **και "Αναγνωριστικό μηνύματος δικτύου".**</span><span class="sxs-lookup"><span data-stu-id="2ca5f-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="2ca5f-104">Ακολουθήστε τα παρακάτω βήματα για να βρείτε το αναγνωριστικό μηνύματος για ένα μήνυμα ηλεκτρονικού ταχυδρομείου στο Outlook:</span><span class="sxs-lookup"><span data-stu-id="2ca5f-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="2ca5f-105">Κάντε διπλό κλικ στο μήνυμα ηλεκτρονικού ταχυδρομείου για να το ανοίξετε.</span><span class="sxs-lookup"><span data-stu-id="2ca5f-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="2ca5f-106">Επιλέξτε **"Ιδιότητες**  >  **αρχείου".**</span><span class="sxs-lookup"><span data-stu-id="2ca5f-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="2ca5f-107">Ανοίξτε το Σημειωματάριο ή ένα κενό έγγραφο του Word και, στη συνέχεια, αντιγράψτε και επικολλήστε το περιεχόμενο που βρίσκεται στο πλαίσιο κεφαλίδων **Internet** στο ανοιχτό έγγραφο για καλύτερη ορατότητα.</span><span class="sxs-lookup"><span data-stu-id="2ca5f-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="2ca5f-108">Εντοπίστε **το πεδίο X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="2ca5f-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="2ca5f-109">Η τιμή μετά το **: είναι** το αναγνωριστικό που χρειάζεστε για την υποβολή σας.</span><span class="sxs-lookup"><span data-stu-id="2ca5f-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="2ca5f-110">Στην **περιοχή "Παραλήπτες",** εάν το μήνυμα ηλεκτρονικού ταχυδρομείου βρίσκεται στο φάκελο ανεπιθύμητης αλληλογραφίας για όλους τους παραλήπτες αυτού του μηνύματος ηλεκτρονικού ταχυδρομείου, επιλέξτε **"Επιλογή όλων".**</span><span class="sxs-lookup"><span data-stu-id="2ca5f-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="2ca5f-111">Εάν όχι, επιλέξτε μόνο το χρήστη που ανέφερε το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="2ca5f-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="2ca5f-112">Στην **περιοχή "Αιτία** υποβολής", εάν επιλέξετε "Θα πρέπει να έχει αποκλειστεί", καθορίστε εάν το μήνυμα θα έχει αποκλειστεί ως ανεπιθύμητη **αλληλογραφία,** ηλεκτρονικό "ψάρεμα" ή "Λογισμικό κακόβουλης λειτουργίας" **και,** στη συνέχεια, επιλέξτε  **"Υποβολή".**</span><span class="sxs-lookup"><span data-stu-id="2ca5f-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="2ca5f-113">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα "Πώς να υποβάλετε ύποπτη ανεπιθύμητη αλληλογραφία, ηλεκτρονικό "ψάρεμα", διευθύνσεις URL και αρχεία στη Microsoft για σάρωση.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="2ca5f-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
