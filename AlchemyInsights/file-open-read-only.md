---
title: Αρχείο ανοιχτό μόνο για ανάγνωση
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813184"
---
# <a name="file-open-read-only"></a><span data-ttu-id="51d5c-102">Αρχείο ανοιχτό μόνο για ανάγνωση</span><span class="sxs-lookup"><span data-stu-id="51d5c-102">File open read-only</span></span>

<span data-ttu-id="51d5c-103">Μπορεί να βρείτε ότι όταν ανοίγετε αρχεία, ανοίγουν ως μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="51d5c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="51d5c-104">Σε ορισμένες περιπτώσεις, αυτό αφορά την πρόσθετη ασφάλεια, όπως όταν ανοίγετε αρχεία από το Internet και άλλες φορές, αυτό μπορεί να οφείλεται σε μια ρύθμιση που μπορεί να αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="51d5c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="51d5c-105">Ακολουθούν ορισμένα σενάρια όπου ένα αρχείο ανοίγει μόνο για ανάγνωση και ορισμένα βήματα που μπορείτε να κάνετε για να το αλλάξετε αυτό.</span><span class="sxs-lookup"><span data-stu-id="51d5c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="51d5c-106">**Το λογισμικό προστασίας από ιούς που διανοίγω προκαλεί το άνοιγμα μόνο για ανάγνωση**</span><span class="sxs-lookup"><span data-stu-id="51d5c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="51d5c-107">Ορισμένα προγράμματα προστασίας από ιούς ενδέχεται να σας προστατεύουν από ενδεχομένως μη ασφαλή αρχεία, ανοίγοντας τα μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="51d5c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="51d5c-108">Ίσως χρειαστεί να επικοινωνήστε με την υπηρεσία παροχής προστασίας από ιούς για να μάθετε πώς μπορείτε να προσαρμόσετε αυτές τις ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="51d5c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="51d5c-109">Το BitDefender, για παράδειγμα, έχει περιεχόμενο σχετικά με την προσθήκη εξαιρέσεων εφαρμογών εδώ: Πώς μπορείτε να προσθέσετε εξαιρέσεις εφαρμογών ή διεργασιών [στο Κέντρο ελέγχου Bitdefender.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="51d5c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="51d5c-110">**Οι ιδιότητες αρχείου έχουν οριστεί σε μόνο για ανάγνωση;**</span><span class="sxs-lookup"><span data-stu-id="51d5c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="51d5c-111">Μπορείτε να ελέγξετε τις ιδιότητες αρχείου κάνοντας δεξί κλικ στο αρχείο και επιλέγοντας "Ιδιότητες".</span><span class="sxs-lookup"><span data-stu-id="51d5c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="51d5c-112">Εάν το χαρακτηριστικό μόνο για ανάγνωση είναι επιλεγμένο, μπορείτε να το καταργήστε και να κάνετε κλικ στο κουμπί OK.</span><span class="sxs-lookup"><span data-stu-id="51d5c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="51d5c-113">**Το περιεχόμενο είναι σε προστατευμένη προβολή**</span><span class="sxs-lookup"><span data-stu-id="51d5c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="51d5c-114">Τα αρχεία από το Internet και από άλλες ενδεχομένως μη ασφαλείς θέσεις μπορεί να περιέχουν ιούς, ιούς τύπου worm ή άλλα είδη κακόβουλης λειτουργίας που μπορεί να βλάψουν τον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="51d5c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="51d5c-115">Αυτό συμβαίνει επίσης συχνά με τα συνημμένα ηλεκτρονικού ταχυδρομείου ή τα αρχεία που έχετε κάνει λήψη.</span><span class="sxs-lookup"><span data-stu-id="51d5c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="51d5c-116">Για την προστασία του υπολογιστή σας, τα αρχεία από αυτές τις ενδεχομένως μη ασφαλείς θέσεις ανοίγουν σε Προστατευμένη προβολή.</span><span class="sxs-lookup"><span data-stu-id="51d5c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="51d5c-117">Χρησιμοποιώντας την Προστατευμένη προβολή, μπορείτε να διαβάσετε ένα αρχείο και να δείτε τα περιεχόμενά του, μειώνοντας παράλληλα τους κινδύνους.</span><span class="sxs-lookup"><span data-stu-id="51d5c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="51d5c-118">Για περισσότερες πληροφορίες σχετικά με την Προστατευμένη προβολή και τον τρόπο αλλαγής ρυθμίσεων, ανατρέξτε σε αυτό το άρθρο: [Τι είναι η Προστατευμένη προβολή;](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="51d5c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="51d5c-119">**Είναι πλήρες το OneDrive;**</span><span class="sxs-lookup"><span data-stu-id="51d5c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="51d5c-120">Εάν το αρχείο είναι αποθηκευμένο στο OneDrive και ο χώρος αποθήκευσης στο OneDrive είναι πλήρης, δεν θα μπορείτε να αποθηκεύσετε το έγγραφο μέχρι να είστε κάτω από τον χώρο που σας έχει παραχωρηθεί.</span><span class="sxs-lookup"><span data-stu-id="51d5c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="51d5c-121">Μπορείτε να ελέγξετε τον ελεύθερο χώρο σας στο OneDrive κάνοντας κλικ στο εικονίδιο του OneDrive στο κέντρο ειδοποιήσεων και επιλέγοντας "Διαχείριση χώρου αποθήκευσης" ή μπορείτε να μεταβείτε στο , να εισέλθετε και να σημειώσετε την ποσότητα του χώρου που χρησιμοποιείται στην κάτω αριστερή γωνία [https://onedrive.live.com](https://onedrive.live.com) της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="51d5c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="51d5c-122">**Είναι ενεργοποιημένο το Office;**</span><span class="sxs-lookup"><span data-stu-id="51d5c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="51d5c-123">Εάν το Office δεν είναι ενεργοποιημένο ή εάν η συνδρομή σας έχει λήξει, μπορεί να είστε σε κατάσταση μειωμένης λειτουργικότητας μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="51d5c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="51d5c-124">Για πληροφορίες σχετικά με τον τρόπο ενεργοποίησης του Office, ανατρέξτε στο θέμα: Σφάλματα "Προϊόν χωρίς άδεια [χρήσης" και σφάλματα ενεργοποίησης στο Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="51d5c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="51d5c-125">**Εάν αποτύχουν όλα τα άλλα...**</span><span class="sxs-lookup"><span data-stu-id="51d5c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="51d5c-126">Δοκιμάστε να επανεκκινήσετε τον υπολογιστή</span><span class="sxs-lookup"><span data-stu-id="51d5c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="51d5c-127">Εγκατάσταση ενημερώσεων του Office</span><span class="sxs-lookup"><span data-stu-id="51d5c-127">Install Office updates</span></span>
    
- <span data-ttu-id="51d5c-128">Εκτέλεση επιδιόρθωσης του Office μέσω Internet</span><span class="sxs-lookup"><span data-stu-id="51d5c-128">Perform an Online repair of Office</span></span>
    

