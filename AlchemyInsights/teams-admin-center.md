---
title: Κέντρο διαχείρισης του Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670364"
---
# <a name="teams-admin-center"></a><span data-ttu-id="4c6bb-102">Κέντρο διαχείρισης του Teams</span><span class="sxs-lookup"><span data-stu-id="4c6bb-102">Teams Admin Center</span></span>

<span data-ttu-id="4c6bb-103">Μάθετε σχετικά με τη διαχείριση του Teams με το [Κέντρο διαχείρισης του Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4c6bb-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="4c6bb-104">Εάν δεν μπορείτε να αποκτήσετε πρόσβαση στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="4c6bb-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="4c6bb-105">Βεβαιωθείτε ότι έχετε επιτρέψει στις κατάλληλες [διευθύνσεις IP και διευθύνσεις URL του Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) σε οποιεσδήποτε περιμετρικές συσκευές (τείχος προστασίας, κ. λπ.) ή στους κανόνες τείχους προστασίας στον τοπικό υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="4c6bb-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="4c6bb-106">Επαληθεύστε ότι η σύνδεση που χρησιμοποιείτε για να αποκτήσετε πρόσβαση στην πύλη διαχείρισης του Teams συμφωνεί με το όνομα χρήστη που αναγράφεται στην [πύλη διαχείρισης του Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="4c6bb-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="4c6bb-107">Εάν δεν εμφανίζονται χρήστες στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα:</span><span class="sxs-lookup"><span data-stu-id="4c6bb-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="4c6bb-108">Έχετε δημιουργήσει χρήστες ή έχετε εκχωρήσει άδειες χρήσης τις τελευταίες 24 ώρες;</span><span class="sxs-lookup"><span data-stu-id="4c6bb-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="4c6bb-109">Φροντίστε να περιμένετε τουλάχιστον 24 ώρες πριν ανοίξετε ένα δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="4c6bb-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="4c6bb-110">Είστε βέβαιοι ότι έχετε εκχωρήσει κατάλληλες άδειες χρήσης;</span><span class="sxs-lookup"><span data-stu-id="4c6bb-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="4c6bb-111">Εάν έχετε μια υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, επαληθεύστε ότι [η τιμή msRTCSIP-PrimaryUserAddress ή η διεύθυνση SIP στο πεδίο proxyAddresses της τοπικής υπηρεσίας καταλόγου Active Directory είναι μοναδική και η μορφή ταιριάζει](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) με SIP: το**όνομα** χρήστη του χρήστη από το [Κέντρο διαχείρισης του Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="4c6bb-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="4c6bb-112">Εάν σκοπεύετε να διατηρήσετε μια ανάπτυξη του Skype για επιχειρήσεις Server και να έχετε χρήστες που διαθέτουν εσωτερικές εγκαταστάσεις και online: ακολουθήστε τις επιλογές **"ρύθμιση υβριδικού με ομάδες και Skype για επιχειρήσεις online"** στον πίνακα ελέγχου του Skype για επιχειρήσεις και μετακινήστε τους χρήστες στο Internet.</span><span class="sxs-lookup"><span data-stu-id="4c6bb-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
