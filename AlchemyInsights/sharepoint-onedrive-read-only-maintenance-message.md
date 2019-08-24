---
title: Μόνο για ανάγνωση για συντήρηση μήνυμα κατά την προσπάθεια χρήσης του SharePoint ή OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620723"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="c72fc-102">Μόνο για ανάγνωση για συντήρηση μήνυμα κατά την προσπάθεια χρήσης του SharePoint ή OneDrive</span><span class="sxs-lookup"><span data-stu-id="c72fc-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="c72fc-103">Χρήστες ενδέχεται να λάβουν ένα μήνυμα **Μόνο για ανάγνωση για συντήρηση** , κατά την προσπάθεια χρήσης του SharePoint ή OneDrive για ένα από τα ακόλουθα σενάρια.</span><span class="sxs-lookup"><span data-stu-id="c72fc-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="c72fc-104">Μια δραστηριότητα προγραμματισμένες ή ενεργό συντήρησης.</span><span class="sxs-lookup"><span data-stu-id="c72fc-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="c72fc-105">Ελέγξτε τους, μεταβαίνοντας στο [Κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="c72fc-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="c72fc-106">Ένα συμβάν ενεργή υπηρεσία υψηλής προτεραιότητας, που ίσως παρουσιάζεται.</span><span class="sxs-lookup"><span data-stu-id="c72fc-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="c72fc-107">Ελέγξτε για τυχόν advisories/συμβάντων στην [Υπηρεσία υγείας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c72fc-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="c72fc-108">Μια δευτερεύουσα Αυτόματης Διόρθωσης σενάριο αποκατάστασης που θα μπορούσε να συμβεί λόγω μη αναμενόμενα συμβάντα στους διακομιστές που μπορεί να διαρκέσει λιγότερο από 30 min ή αυτό.</span><span class="sxs-lookup"><span data-stu-id="c72fc-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="c72fc-109">Υπάρχουν δεν Κέντρο μηνυμάτων ή υπηρεσία υγείας καταχωρεί αυτές τις δευτερεύουσες ανακτήσεις αλλά θα πρέπει να Επιστροφή στην κανονική πολύ σύντομα.</span><span class="sxs-lookup"><span data-stu-id="c72fc-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="c72fc-110">Πολύ λίγες φορές μας παρατηρείται ότι μία από τις τρεις περιπτώσεις που παρατίθενται παραπάνω έχουν την αιτία, και έχει γίνει η επαναφορά της υπηρεσίας, αλλά δεν έχει καταργηθεί από τη μνήμη cache του προγράμματος περιήγησης στους χρήστες προς τα επάνω.</span><span class="sxs-lookup"><span data-stu-id="c72fc-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="c72fc-111">Προσπαθήστε να απενεργοποιήσετε τη μνήμη cache του προγράμματος περιήγησης πριν από την περιήγηση στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="c72fc-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="c72fc-112">Στο πρόγραμμα περιήγησης Microsoft άκρη, επιλέξτε **Ρυθμίσεις**και, στη συνέχεια, επιλέξτε **απόρρητο και την ασφάλεια**.</span><span class="sxs-lookup"><span data-stu-id="c72fc-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="c72fc-113">Στην περιοχή **Απαλοιφή περιήγηση**, επιλέξτε **Επιλέξτε τι πρέπει να καταργήσετε την επιλογή**.</span><span class="sxs-lookup"><span data-stu-id="c72fc-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="c72fc-114">Επιλέξτε **Τα Cookies και δεδομένων αποθηκευμένων τοποθεσιών Web**και επιλέξτε **Clear**.</span><span class="sxs-lookup"><span data-stu-id="c72fc-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="c72fc-115">Αυτά τα βήματα ενδέχεται να διαφέρουν όταν χρησιμοποιείτε άλλα προγράμματα περιήγησης όπως Mozilla Firefox ή Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="c72fc-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="c72fc-116">Μια άλλη επιλογή είναι να ανοίξετε την τοποθεσία του SharePoint ή OneDrive σε ένα νέο παράθυρο InPrivate.</span><span class="sxs-lookup"><span data-stu-id="c72fc-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>