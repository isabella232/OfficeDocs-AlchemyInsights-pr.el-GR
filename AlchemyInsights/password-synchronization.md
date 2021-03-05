---
title: Συγχρονισμός κωδικού πρόσβασης
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481447"
---
# <a name="password-synchronization"></a><span data-ttu-id="b5a5c-102">Συγχρονισμός κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="b5a5c-102">Password synchronization</span></span>

<span data-ttu-id="b5a5c-103">**Ο συγχρονισμός hash κωδικού πρόσβασης δεν λειτουργεί καθόλου**</span><span class="sxs-lookup"><span data-stu-id="b5a5c-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="b5a5c-104">Ορισμένα συνήθη προβλήματα που αντιμετωπίζουν οι πελάτες όταν ο συγχρονισμός του hash κωδικού πρόσβασης δεν λειτουργεί είναι:</span><span class="sxs-lookup"><span data-stu-id="b5a5c-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="b5a5c-105">Στο λογαριασμό της υπηρεσίας καταλόγου Active Directory που χρησιμοποιείται από το Azure AD  Connect για την επικοινωνία με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης δεν εκχωρείται η δυνατότητα **"Αναπαραγωγή** αλλαγών καταλόγου" και "Αναπαραγωγή καταλόγου αλλαγών όλα τα δικαιώματα", τα οποία απαιτούνται για το συγχρονισμό κωδικού πρόσβασης - Πρέπει να το διορθώσετε αυτό εκχωρώντας αυτά τα δικαιώματα στο λογαριασμό της υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="b5a5c-106">Ο συγχρονισμός hash κωδικού πρόσβασης απενεργοποιείται όταν  ένας διαχειριστής άλλαξε τη μέθοδο user Sign-In από συγχρονισμό κωδικού πρόσβασης σε μια άλλη επιλογή, όπως "Ομοσπονδία με **υπηρεσίες AD FS"** στον Οδηγό Azure AD Connect - Μπορείτε να διορθώσετε αυτό το πρόβλημα ενεργοποιώντας εκ πάλι τη δυνατότητα συγχρονισμού **hash κωδικού** πρόσβασης στον οδηγό Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="b5a5c-107">Πρόβλημα συνδεσιμότητας με την υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="b5a5c-108">Για παράδειγμα, ορισμένοι ελεγκτές τομέα δεν είναι προσβάσιμοι [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) από το Azure AD Connect ή οι θύρες που απαιτούνται έχουν αποκλειστεί από το τείχος προστασίας . Πρέπει να διορθώσετε αυτό το πρόβλημα εξασφαλίζοντας ότι η σύνδεση μεταξύ του διακομιστή Azure AD Connect και της υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης λειτουργεί σωστά.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="b5a5c-109">Ο διακομιστής Azure AD Connect βρίσκεται αυτή τη στιγμή σε κατάσταση λειτουργίας προέκτασης, γεγονός που θα έχει ως αποτέλεσμα ο διακομιστής να μην έχει τη δυνατότητα να κάνει hashehes τον κωδικό πρόσβασης - Για να αντιμετωπίσετε το πρόβλημα, ακολουθήστε τα βήματα που περιγράφονται στην ενότητα Αντιμετώπιση προβλημάτων συγχρονισμού κωδικών πρόσβασης με συγχρονισμό [Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Δεν συγχρονίζονται κωδικοί πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="b5a5c-110">**Ο συγχρονισμός hash κωδικού πρόσβασης δεν λειτουργεί για ορισμένους από τους χρήστες μου**</span><span class="sxs-lookup"><span data-stu-id="b5a5c-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="b5a5c-111">Εάν παρατηρήσατε ότι ο hash κωδικού πρόσβασης δεν  συγχρονίζεται για ένα χρήστη, χρησιμοποιήστε την εργασία αντιμετώπισης προβλημάτων στο Azure AD Connect για να διερευνήσετε και να επιλύσετε το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="b5a5c-112">Εκτέλεση των ακόλουθων εργασιών:</span><span class="sxs-lookup"><span data-stu-id="b5a5c-112">Perform the following tasks:</span></span>

    <span data-ttu-id="b5a5c-113">a.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-113">a.</span></span> [<span data-ttu-id="b5a5c-114">Εκτέλεση της εργασίας αντιμετώπισης προβλημάτων στον οδηγό</span><span class="sxs-lookup"><span data-stu-id="b5a5c-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="b5a5c-115">b.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-115">b.</span></span> [<span data-ttu-id="b5a5c-116">Χρησιμοποιήστε το cmdlet αντιμετώπισης προβλημάτων για να διερευνήσετε το πρόβλημα συγχρονισμού του hash κωδικού πρόσβασης για μια συγκεκριμένη χρήση</span><span class="sxs-lookup"><span data-stu-id="b5a5c-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="b5a5c-117">Το αντικείμενο χρήστη της υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης είναι ενεργοποιημένο για τον **χρήστη πρέπει να αλλάξει τον κωδικό πρόσβασης κατά την επόμενη επιλογή** σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="b5a5c-118">Όταν αυτή η επιλογή είναι ενεργοποιημένη, στο χρήστη εκχωρείται ένας προσωρινός κωδικός πρόσβασης και θα του ζητηθεί να αλλάξει τον κωδικό πρόσβασης κατά την επόμενη σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="b5a5c-119">Το Azure AD Connect δεν συγχρονίζει προσωρινούς κωδικούς πρόσβασης στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="b5a5c-120">Για να επιλύσετε το παραπάνω ζήτημα, εκτελέστε μία από τις ακόλουθες εργασίες:</span><span class="sxs-lookup"><span data-stu-id="b5a5c-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="b5a5c-121">Ζητήστε από το χρήστη να κάνει είσοδο στην εφαρμογή εσωτερικής εγκατάστασης (για παράδειγμα, στην επιφάνεια εργασίας των Windows) και να αλλάξει τον κωδικό πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="b5a5c-122">Ο νέος κωδικός πρόσβασης θα συγχρονιστεί στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="b5a5c-123">Εάν ένας διαχειριστής ενημερώσει τον κωδικό πρόσβασης του χρήστη χωρίς να ενεργοποιήσετε την επιλογή, ο χρήστης πρέπει να αλλάξει τον κωδικό πρόσβασης κατά την επόμενη σύνδεση και να μοιραστεί τον νέο κωδικό πρόσβασης με τον χρήστη.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="b5a5c-124">Το αντικείμενο χρήστη της υπηρεσίας καταλόγου Active Directory εσωτερικής εγκατάστασης δεν **έχει ρυθμιστεί σωστά για συγχρονισμό** αντικειμένων ή συγχρονισμό κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="b5a5c-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="b5a5c-125">Για να αντιμετωπίσετε αυτό το πρόβλημα, ακολουθήστε τα βήματα που περιγράφονται στο θέμα Αντιμετώπιση προβλημάτων συγχρονισμού [hash κωδικού πρόσβασης με το συγχρονισμό Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="b5a5c-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







