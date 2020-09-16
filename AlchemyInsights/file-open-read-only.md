---
title: Άνοιγμα αρχείου μόνο για ανάγνωση
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745583"
---
# <a name="file-open-read-only"></a><span data-ttu-id="3e933-102">Άνοιγμα αρχείου μόνο για ανάγνωση</span><span class="sxs-lookup"><span data-stu-id="3e933-102">File open read-only</span></span>

<span data-ttu-id="3e933-103">Μπορεί να διαπιστώσετε ότι, όταν ανοίγετε αρχεία, ανοίγουν μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="3e933-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="3e933-104">Σε ορισμένες περιπτώσεις, αυτό ισχύει για πρόσθετη ασφάλεια, όπως όταν ανοίγετε αρχεία από το Internet και άλλες φορές, μπορεί να οφείλεται σε μια ρύθμιση που μπορεί να αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="3e933-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="3e933-105">Ακολουθούν ορισμένα σενάρια όπου ένα αρχείο ανοίγει μόνο για ανάγνωση και ορισμένα βήματα που μπορείτε να ακολουθήσετε για να το αλλάξετε.</span><span class="sxs-lookup"><span data-stu-id="3e933-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="3e933-106">**Το antivirus μου τους προκαλεί να ανοίγουν μόνο για ανάγνωση**</span><span class="sxs-lookup"><span data-stu-id="3e933-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="3e933-107">Ορισμένα προγράμματα προστασίας από ιούς ενδέχεται να σας προστατεύουν από πιθανώς μη ασφαλή αρχεία, ανοίγοντας τα μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="3e933-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="3e933-108">Ίσως χρειαστεί να επικοινωνήσετε με την υπηρεσία παροχής προστασίας από ιούς για να μάθετε πώς μπορείτε να προσαρμόσετε αυτές τις ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="3e933-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="3e933-109">Το BitDefender, για παράδειγμα, έχει περιεχόμενο σχετικά με την προσθήκη εξαιρέσεων εφαρμογών εδώ: [Πώς να προσθέσετε εξαιρέσεις εφαρμογών ή διεργασιών στο κέντρο ελέγχου BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="3e933-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="3e933-110">**Οι ιδιότητες αρχείου έχουν την τιμή "μόνο για ανάγνωση";**</span><span class="sxs-lookup"><span data-stu-id="3e933-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="3e933-111">Μπορείτε να επιλέξετε τις ιδιότητες αρχείου κάνοντας δεξί κλικ στο αρχείο και επιλέγοντας ιδιότητες.</span><span class="sxs-lookup"><span data-stu-id="3e933-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="3e933-112">Εάν είναι επιλεγμένο το χαρακτηριστικό μόνο για ανάγνωση, μπορείτε να το καταργήσετε και να κάνετε κλικ στο κουμπί OK.</span><span class="sxs-lookup"><span data-stu-id="3e933-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="3e933-113">**Το περιεχόμενο βρίσκεται σε προστατευμένη προβολή**</span><span class="sxs-lookup"><span data-stu-id="3e933-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="3e933-114">Τα αρχεία από το Internet και από άλλες δυνητικά μη ασφαλείς θέσεις μπορεί να περιέχουν ιούς, ιούς τύπου worm ή άλλα είδη κακόβουλου λογισμικού που μπορούν να βλάψουν τον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="3e933-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="3e933-115">Αυτό συμβαίνει επίσης συνήθως με τα συνημμένα ηλεκτρονικού ταχυδρομείου ή τα αρχεία που έχετε λάβει.</span><span class="sxs-lookup"><span data-stu-id="3e933-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="3e933-116">Για την προστασία του υπολογιστή σας, τα αρχεία από αυτές τις δυνητικά μη ασφαλείς θέσεις ανοίγουν σε προστατευμένη προβολή.</span><span class="sxs-lookup"><span data-stu-id="3e933-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="3e933-117">Χρησιμοποιώντας την προστατευμένη προβολή, μπορείτε να διαβάσετε ένα αρχείο και να δείτε τα περιεχόμενά του μειώνοντας τους κινδύνους.</span><span class="sxs-lookup"><span data-stu-id="3e933-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="3e933-118">Για περισσότερες πληροφορίες σχετικά με την προστατευμένη προβολή και τον τρόπο αλλαγής των ρυθμίσεων, ανατρέξτε σε αυτό το άρθρο: [Τι είναι η προστατευμένη προβολή;](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="3e933-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="3e933-119">**Είναι πλήρες το OneDrive;**</span><span class="sxs-lookup"><span data-stu-id="3e933-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="3e933-120">Εάν το αρχείο είναι αποθηκευμένο στο OneDrive και ο χώρος αποθήκευσης του OneDrive είναι πλήρης, δεν θα μπορείτε να αποθηκεύσετε το έγγραφο μέχρι να είστε κάτω από τον επιτρεπόμενο χώρο σας.</span><span class="sxs-lookup"><span data-stu-id="3e933-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="3e933-121">Μπορείτε να κάνετε έλεγχο του ελεύθερου χώρου σας στο OneDrive, κάνοντας κλικ στο εικονίδιο του OneDrive στο κέντρο ειδοποιήσεων και επιλέγοντας Διαχείριση χώρου αποθήκευσης ή μπορείτε να μεταβείτε στο [https://onedrive.live.com](https://onedrive.live.com) , να εισέλθετε και να σημειώσετε την ποσότητα του χρησιμοποιημένου χώρου στο κάτω αριστερό μέρος της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="3e933-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="3e933-122">**Είναι ενεργοποιημένο το Office;**</span><span class="sxs-lookup"><span data-stu-id="3e933-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="3e933-123">Εάν το Office δεν είναι ενεργοποιημένο ή εάν η συνδρομή σας έχει λήξει, μπορεί να βρίσκεστε σε κατάσταση μειωμένης λειτουργικότητας μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="3e933-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="3e933-124">Για πληροφορίες σχετικά με τον τρόπο ενεργοποίησης του Office, ανατρέξτε στο θέμα: [σφάλματα προϊόντος και ενεργοποίησης χωρίς άδεια χρήσης στο Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3e933-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="3e933-125">**Εάν όλα τα άλλα αποτύχουν...**</span><span class="sxs-lookup"><span data-stu-id="3e933-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="3e933-126">Δοκιμάστε να επανεκκινήσετε τον υπολογιστή</span><span class="sxs-lookup"><span data-stu-id="3e933-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="3e933-127">Εγκατάσταση ενημερώσεων του Office</span><span class="sxs-lookup"><span data-stu-id="3e933-127">Install Office updates</span></span>
    
- <span data-ttu-id="3e933-128">Εκτέλεση ηλεκτρονικής επιδιόρθωσης του Office</span><span class="sxs-lookup"><span data-stu-id="3e933-128">Perform an Online repair of Office</span></span>
    

