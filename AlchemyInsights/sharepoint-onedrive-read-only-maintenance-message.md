---
title: Μόνο για ανάγνωση του μηνύματος συντήρησης κατά την προσπάθεια χρήσης του SharePoint ή του OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051281"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="6b36a-102">Μόνο για ανάγνωση του μηνύματος συντήρησης κατά την προσπάθεια χρήσης του SharePoint ή του OneDrive</span><span class="sxs-lookup"><span data-stu-id="6b36a-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="6b36a-103">Οι χρήστες ενδέχεται να λάβετε ένα μήνυμα **μόνο για ανάγνωση για συντήρηση** όταν επιχειρείτε να χρησιμοποιήσετε το SharePoint ή το OneDrive για ένα από τα ακόλουθα σενάρια.</span><span class="sxs-lookup"><span data-stu-id="6b36a-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="6b36a-104">Μια προγραμματισμένη ή ενεργή δραστηριότητα συντήρησης.</span><span class="sxs-lookup"><span data-stu-id="6b36a-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="6b36a-105">Ελέγξτε για αυτούς μεταβαίνοντας στο [Κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="6b36a-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="6b36a-106">Ένα περιστατικό υψηλής προτεραιότητας, ενεργού υπηρεσίας που μπορεί να συμβεί.</span><span class="sxs-lookup"><span data-stu-id="6b36a-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="6b36a-107">Ελέγξτε για τυχόν προειδοποιήσεις/συμβάντα μεταβαίνοντας στην [υπηρεσία εύρυθμης λειτουργίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6b36a-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="6b36a-108">Ένα μικρό σενάριο ανάκτησης αυτόματης αποκατάστασης που θα μπορούσε να συμβεί λόγω τυχόν απροσδόκητων συμβάντων στους διακομιστές που μπορεί να διαρκέσει για λιγότερο από 30 λεπτά ή έτσι.</span><span class="sxs-lookup"><span data-stu-id="6b36a-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="6b36a-109">Δεν υπάρχουν αναρτήσεις στο κέντρο μηνυμάτων ή στην υπηρεσία εύρυθμης λειτουργίας για αυτές τις δευτερεύουσες ανακτήσεις, αλλά θα πρέπει να είστε πάλι φυσιολογικοί πολύ σύντομα.</span><span class="sxs-lookup"><span data-stu-id="6b36a-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="6b36a-110">Σε πολύ λίγες περιπτώσεις παρατηρήσαμε ότι ένα από τα τρία σενάρια που αναφέρονται παραπάνω ήταν η αιτία και η υπηρεσία αποκαταστάθηκε, αλλά η μνήμη cache του προγράμματος περιήγησης των χρηστών δεν έχει ξεκαθαρίσει.</span><span class="sxs-lookup"><span data-stu-id="6b36a-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="6b36a-111">Προσπαθήστε να καταργήσετε τη μνήμη cache του προγράμματος περιήγησης πριν από την πλοήγηση στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="6b36a-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="6b36a-112">Στο πρόγραμμα περιήγησης Microsoft Edge, επιλέξτε **Ρυθμίσεις**και, στη συνέχεια, επιλέξτε **προστασία προσωπικών δεδομένων και ασφάλεια**.</span><span class="sxs-lookup"><span data-stu-id="6b36a-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="6b36a-113">Στην περιοχή **σαφής περιήγηση**, επιλέξτε **Τι θα διαγράψετε**.</span><span class="sxs-lookup"><span data-stu-id="6b36a-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="6b36a-114">Επιλέξτε **cookie και αποθηκευμένα δεδομένα ιστότοπου**και επιλέξτε **Απαλοιφή**.</span><span class="sxs-lookup"><span data-stu-id="6b36a-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="6b36a-115">Αυτά τα βήματα ενδέχεται να διαφέρουν κατά τη χρήση άλλων προγραμμάτων περιήγησης, όπως το Mozilla Firefox ή το Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="6b36a-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="6b36a-116">Μια άλλη επιλογή θα ήταν να ανοίξετε την τοποθεσία SharePoint ή το OneDrive σε ένα νέο παράθυρο InPrivate.</span><span class="sxs-lookup"><span data-stu-id="6b36a-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>