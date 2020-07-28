---
title: Το πιστοποιητικό push της Apple MDM δεν έχει ρυθμιστεί
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439385"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="88d81-102">Το πιστοποιητικό push της Apple MDM δεν έχει ρυθμιστεί</span><span class="sxs-lookup"><span data-stu-id="88d81-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="88d81-103">Ένα πιστοποιητικό push της Apple MDM (γνωστό και ως πιστοποιητικό υπηρεσίας ειδοποιήσεων push της Apple (APNS) δεν έχει ρυθμιστεί για τη συνδρομή σας.</span><span class="sxs-lookup"><span data-stu-id="88d81-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="88d81-104">Χωρίς ρυθμισμένο ένα πιστοποιητικό push Apple MDM, δεν μπορείτε να εγγραφείτε και να διαχειριστείτε συσκευές iOS και Mac OS.</span><span class="sxs-lookup"><span data-stu-id="88d81-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="88d81-105">Αφού προσθέσετε το πιστοποιητικό στο Intune, οι χρήστες μπορούν να εγκαταστήσουν την εφαρμογή Εταιρική πύλη για να εγγράψουν τις συσκευές iOS τους.</span><span class="sxs-lookup"><span data-stu-id="88d81-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="88d81-106">Επιλέξτε **"Συμφωνώ".**</span><span class="sxs-lookup"><span data-stu-id="88d81-106">Select **"I agree."**</span></span> <span data-ttu-id="88d81-107">για να δώσετε στη Microsoft το δικαίωμα να στείλει δεδομένα στην Apple.</span><span class="sxs-lookup"><span data-stu-id="88d81-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="88d81-108">Επιλέξτε **Λήψη του CSR που** απαιτείται από την αίτηση υπογραφής πιστοποιητικού Intune που απαιτείται για τη δημιουργία ενός πιστοποιητικού push Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="88d81-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="88d81-109">Το αρχείο χρησιμοποιείται για την αίτηση πιστοποιητικού σχέσης αξιοπιστίας από την πύλη πιστοποιητικών push της Apple.</span><span class="sxs-lookup"><span data-stu-id="88d81-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="88d81-110">Επιλέξτε **Δημιουργία πιστοποιητικού ώθησης MDM** για να μεταβείτε στην πύλη πιστοποιητικών push της Apple.</span><span class="sxs-lookup"><span data-stu-id="88d81-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="88d81-111">Συνδεθείτε με το Apple ID της εταιρείας σας και, στη συνέχεια, επιλέξτε **Δημιουργία πιστοποιητικού**.</span><span class="sxs-lookup"><span data-stu-id="88d81-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="88d81-112">Επιλέξτε **Επιλογή αρχείου**, αναζητήστε το αρχείο αίτησης υπογραφής πιστοποιητικού και, στη συνέχεια, επιλέξτε **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="88d81-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="88d81-113">Στη σελίδα Επιβεβαίωση, επιλέξτε **Λήψη** για να κάνετε λήψη του αρχείου πιστοποιητικού (.pem) και να αποθηκεύσετε το αρχείο τοπικά.</span><span class="sxs-lookup"><span data-stu-id="88d81-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="88d81-114">**Σημείωση**: Το πιστοποιητικό σχετίζεται με το Apple ID που χρησιμοποιείται για τη δημιουργία του.</span><span class="sxs-lookup"><span data-stu-id="88d81-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="88d81-115">Ως βέλτιστη πρακτική, χρησιμοποιήστε ένα Apple ID εταιρείας για εργασίες διαχείρισης και βεβαιωθείτε ότι το γραμματοκιβώτιο παρακολουθείται από περισσότερα από ένα άτομα ή χρησιμοποιώντας μια λίστα διανομής.</span><span class="sxs-lookup"><span data-stu-id="88d81-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="88d81-116">Μην χρησιμοποιείτε ποτέ προσωπικό Apple ID.</span><span class="sxs-lookup"><span data-stu-id="88d81-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="88d81-117">Χρησιμοποιήστε το ίδιο Apple ID για να ανανεώνετε το Πιστοποιητικό Push της Apple κάθε 12 μήνες.</span><span class="sxs-lookup"><span data-stu-id="88d81-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="88d81-118">Εισαγάγετε το Apple ID που χρησιμοποιήθηκε για τη δημιουργία του πιστοποιητικού ώθησης Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="88d81-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="88d81-119">Καταγράψτε αυτό το αναγνωριστικό ως υπενθύμιση για το πότε πρέπει να ανανεώσετε το πιστοποιητικό.</span><span class="sxs-lookup"><span data-stu-id="88d81-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="88d81-120">Μεταβείτε στο αρχείο πιστοποιητικού (.pem), επιλέξτε **Άνοιγμα**και, στη συνέχεια, επιλέξτε **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="88d81-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="88d81-121">Με το πιστοποιητικό ώθησης, το Intune μπορεί να εγγράψει και να διαχειριστεί συσκευές Apple.</span><span class="sxs-lookup"><span data-stu-id="88d81-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>