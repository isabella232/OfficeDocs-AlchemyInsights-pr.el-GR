---
title: Το αρχείο ανοίγει μόνο για ανάγνωση
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: 4c774864a03b7dbc099f64b7906fa4a0bc26c63c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525738"
---
# <a name="file-open-read-only"></a><span data-ttu-id="b1faa-102">Το αρχείο ανοίγει μόνο για ανάγνωση</span><span class="sxs-lookup"><span data-stu-id="b1faa-102">File open read-only</span></span>

<span data-ttu-id="b1faa-103">Ενδέχεται να διαπιστώσετε ότι όταν ανοίγετε αρχεία, ανοίγουν ως μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="b1faa-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="b1faa-104">Σε ορισμένες περιπτώσεις, αυτό είναι για πρόσθετη ασφάλεια, όπως όταν ανοίγετε αρχεία από το internet και άλλες φορές, αυτό μπορεί να οφείλεται σε μια ρύθμιση που μπορεί να αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="b1faa-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="b1faa-105">Παρακάτω δίνονται ορισμένα σενάρια όπου ένα αρχείο ανοίγει μόνο για ανάγνωση και ορισμένα βήματα που μπορείτε να ακολουθήσετε για να το αλλάξετε.</span><span class="sxs-lookup"><span data-stu-id="b1faa-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="b1faa-106">**Μου το λογισμικό προστασίας από ιούς προκαλεί να ανοίξετε μόνο για ανάγνωση**</span><span class="sxs-lookup"><span data-stu-id="b1faa-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="b1faa-107">Ορισμένα προγράμματα αντιμετώπισης ιών μπορεί να προστατευτείτε από πιθανώς μη ασφαλή αρχεία από το άνοιγμά τους μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="b1faa-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="b1faa-108">Ίσως χρειαστεί να επικοινωνήσετε με τον προμηθευτή του λογισμικού σας για να μάθετε πώς μπορείτε να προσαρμόσετε αυτές τις ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="b1faa-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="b1faa-109">Το BitDefender, για παράδειγμα, έχει περιεχόμενο σχετικά με την προσθήκη εξαιρέσεων εφαρμογή εδώ: [Τρόπος προσθήκης εφαρμογής ή διαδικασίας εξαιρέσεις στο κέντρο ελέγχου Bitdefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="b1faa-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="b1faa-110">**Οι ιδιότητες αρχείου ορίζονται ως μόνο για ανάγνωση;**</span><span class="sxs-lookup"><span data-stu-id="b1faa-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="b1faa-111">Μπορείτε να ελέγξετε τις ιδιότητες του αρχείου, κάνοντας δεξιό κλικ στο αρχείο και επιλέγοντας την εντολή Ιδιότητες.</span><span class="sxs-lookup"><span data-stu-id="b1faa-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="b1faa-112">Εάν είναι ενεργοποιημένο το χαρακτηριστικό μόνο για ανάγνωση, μπορείτε να καταργήσετε την επιλογή του και κάντε κλικ στο κουμπί OK.</span><span class="sxs-lookup"><span data-stu-id="b1faa-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="b1faa-113">**Το περιεχόμενο είναι σε προστατευμένη προβολή**</span><span class="sxs-lookup"><span data-stu-id="b1faa-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="b1faa-114">Αρχεία από το Internet και από άλλες πιθανές μη ασφαλείς θέσεις μπορεί να περιέχουν ιούς, ιούς τύπου worm ή άλλα είδη κακόβουλου λογισμικού που μπορεί να βλάψει τον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="b1faa-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="b1faa-115">Αυτό συμβαίνει επίσης συχνά με συνημμένα σε μηνύματα e-mail ή τα αρχεία που έχετε λάβει.</span><span class="sxs-lookup"><span data-stu-id="b1faa-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="b1faa-116">Για να προστατεύσετε τον υπολογιστή σας, τα αρχεία από αυτές τις πιθανές μη ασφαλείς θέσεις ανοίγουν σε προστατευμένη προβολή.</span><span class="sxs-lookup"><span data-stu-id="b1faa-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="b1faa-117">Χρησιμοποιώντας την προστατευμένη προβολή, μπορείτε να διαβάσετε ένα αρχείο και να δείτε τα περιεχόμενά του κατά τη μείωση των κινδύνων.</span><span class="sxs-lookup"><span data-stu-id="b1faa-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="b1faa-118">Για περισσότερες πληροφορίες σχετικά με την προστατευμένη προβολή και πώς μπορείτε να αλλάξετε τις ρυθμίσεις, ανατρέξτε στην ενότητα αυτού του άρθρου: [Τι είναι η προστατευμένη προβολή;](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="b1faa-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="b1faa-119">**Είναι πλήρης OneDrive;**</span><span class="sxs-lookup"><span data-stu-id="b1faa-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="b1faa-120">Εάν το αρχείο είναι αποθηκευμένο σε OneDrive και το χώρο αποθήκευσης του OneDrive σας είναι πλήρης, δεν θα μπορείτε να αποθηκεύσετε το έγγραφο, μέχρι να είναι στην περιοχή του χώρου που έχει παραχωρηθεί.</span><span class="sxs-lookup"><span data-stu-id="b1faa-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="b1faa-121">Μπορείτε να ελέγξετε τον ελεύθερο χώρο στο OneDrive, κάνοντας κλικ στο εικονίδιο OneDrive στο κέντρο ειδοποιήσεων και επιλέγοντας Διαχείριση αποθήκευσης ή μπορείτε να μεταβείτε στην [http://onedrive.live.com](http://onedrive.live.com), εισέλθετε και σημειώστε την ποσότητα χώρου που χρησιμοποιείται στο κάτω αριστερά μέρος της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="b1faa-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="b1faa-122">**Office έχει ενεργοποιηθεί;**</span><span class="sxs-lookup"><span data-stu-id="b1faa-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="b1faa-123">Εάν δεν έχει ενεργοποιηθεί το Office ή εάν η συνδρομή σας έχει λήξει, μπορεί να είστε σε κατάσταση μόνο για ανάγνωση κατάσταση μειωμένης λειτουργικότητας.</span><span class="sxs-lookup"><span data-stu-id="b1faa-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="b1faa-124">Για πληροφορίες σχετικά με τον τρόπο ενεργοποίησης του Office, ανατρέξτε στο θέμα: [προϊόν χωρίς άδεια χρήσης και σφαλμάτων ενεργοποίησης του Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="b1faa-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="b1faa-125">**Εάν όλα έχουν αποτύχει...**</span><span class="sxs-lookup"><span data-stu-id="b1faa-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="b1faa-126">Προσπαθήστε να ξεκινήσετε πάλι τον υπολογιστή</span><span class="sxs-lookup"><span data-stu-id="b1faa-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="b1faa-127">Εγκατάσταση ενημερωμένων εκδόσεων του Office</span><span class="sxs-lookup"><span data-stu-id="b1faa-127">Install Office updates</span></span>
    
- <span data-ttu-id="b1faa-128">Εκτελέστε μια ηλεκτρονική επιδιόρθωση του Office</span><span class="sxs-lookup"><span data-stu-id="b1faa-128">Perform an Online repair of Office</span></span>
    

