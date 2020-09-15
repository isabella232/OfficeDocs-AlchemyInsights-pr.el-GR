---
title: Μήνυμα "μόνο για ανάγνωση" για συντήρηση όταν προσπαθείτε να χρησιμοποιήσετε το SharePoint ή το OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670832"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="b4dc2-102">Μήνυμα "μόνο για ανάγνωση" για συντήρηση όταν προσπαθείτε να χρησιμοποιήσετε το SharePoint ή το OneDrive</span><span class="sxs-lookup"><span data-stu-id="b4dc2-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="b4dc2-103">Οι χρήστες ενδέχεται να λάβουν ένα μήνυμα **συντήρησης μόνο για ανάγνωση,** όταν επιχειρούν να χρησιμοποιήσουν το SharePoint ή το OneDrive για ένα από τα παρακάτω σενάρια.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="b4dc2-104">Μια προγραμματισμένη ή ενεργή δραστηριότητα συντήρησης.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="b4dc2-105">Αναζητήστε τα με την περιήγηση στο [Κέντρο μηνυμάτων](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="b4dc2-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="b4dc2-106">Ένα περιστατικό υψηλής προτεραιότητας, ενεργού υπηρεσίας που ενδέχεται να προκύψει.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="b4dc2-107">Αναζητήστε τυχόν συμβουλές/περιστατικά με περιήγηση στην [εύρυθμη λειτουργία των υπηρεσιών](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b4dc2-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="b4dc2-108">Ένα μικρό σενάριο αποκατάστασης αυτόματης αποκατάστασης που μπορεί να συμβαίνει εξαιτίας τυχόν μη αναμενόμενων συμβάντων στους διακομιστές που μπορεί να διαρκέσουν λιγότερο από 30 λεπτά περίπου.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="b4dc2-109">Δεν υπάρχουν κέντρα μηνυμάτων ή θέσεις εύρυθμης λειτουργίας υπηρεσιών για αυτές τις δευτερεύουσες ανακτήσεις, αλλά θα πρέπει να επιστρέψετε στο κανονικό πολύ σύντομα.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="b4dc2-110">Σε πολύ λίγες περιπτώσεις παρατηρήσαμε ότι ένα από τα τρία σενάρια που αναφέρονται παραπάνω έχουν την αιτία και η υπηρεσία έχει αποκατασταθεί, αλλά η μνήμη cache του προγράμματος περιήγησης των χρηστών δεν έχει εκκαθαριστεί.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="b4dc2-111">Προσπαθήστε να απαλείψετε το cache του προγράμματος περιήγησης πριν από την περιήγηση στην τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="b4dc2-112">Στο πρόγραμμα περιήγησής σας στο Microsoft Edge, επιλέξτε **Ρυθμίσεις**και, στη συνέχεια, επιλέξτε **προστασία προσωπικών δεδομένων και ασφάλεια**.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="b4dc2-113">Στην περιοχή **Εκκαθάριση περιήγησης**, επιλέξτε **επιλογή των στοιχείων που θα απαλείψετε**.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="b4dc2-114">Επιλέξτε **cookies και αποθηκευμένα δεδομένα ιστότοπου**και επιλέξτε **Απαλοιφή**.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="b4dc2-115">Αυτά τα βήματα ενδέχεται να διαφέρουν κατά τη χρήση άλλων προγραμμάτων περιήγησης, όπως το Mozilla Firefox ή το Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="b4dc2-116">Μια άλλη επιλογή θα ήταν να ανοίξετε την τοποθεσία του SharePoint ή το OneDrive σε ένα νέο παράθυρο InPrivate.</span><span class="sxs-lookup"><span data-stu-id="b4dc2-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>