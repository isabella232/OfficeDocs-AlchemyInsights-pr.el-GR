---
title: Κέντρο διαχείρισης του Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826379"
---
# <a name="teams-admin-center"></a><span data-ttu-id="9c6ee-102">Κέντρο διαχείρισης του Teams</span><span class="sxs-lookup"><span data-stu-id="9c6ee-102">Teams Admin Center</span></span>

<span data-ttu-id="9c6ee-103">Μάθετε σχετικά με τη διαχείριση του Teams με το [Κέντρο διαχείρισης του Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="9c6ee-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="9c6ee-104">Εάν δεν μπορείτε να αποκτήσετε πρόσβαση στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="9c6ee-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="9c6ee-105">Βεβαιωθείτε ότι έχετε επιτρέψει στις κατάλληλες [διευθύνσεις IP και διευθύνσεις URL του Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) σε οποιεσδήποτε περιμετρικές συσκευές (τείχος προστασίας, κ. λπ.) ή στους κανόνες τείχους προστασίας στον τοπικό υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="9c6ee-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="9c6ee-106">Επαληθεύστε ότι η σύνδεση που χρησιμοποιείτε για να αποκτήσετε πρόσβαση στην πύλη διαχείρισης του Teams συμφωνεί με το όνομα χρήστη που αναγράφεται στην [πύλη διαχείρισης του Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="9c6ee-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="9c6ee-107">Εάν δεν εμφανίζονται χρήστες στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα:</span><span class="sxs-lookup"><span data-stu-id="9c6ee-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="9c6ee-108">Έχετε δημιουργήσει χρήστες ή έχετε εκχωρήσει άδειες χρήσης τις τελευταίες 24 ώρες;</span><span class="sxs-lookup"><span data-stu-id="9c6ee-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="9c6ee-109">Φροντίστε να περιμένετε τουλάχιστον 24 ώρες πριν ανοίξετε ένα δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="9c6ee-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="9c6ee-110">Είστε βέβαιοι ότι έχετε εκχωρήσει κατάλληλες άδειες χρήσης;</span><span class="sxs-lookup"><span data-stu-id="9c6ee-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="9c6ee-111">Εάν έχετε μια υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, βεβαιωθείτε ότι η τιμή [του msRTCSIP-PrimaryUserAddress ή της διεύθυνσης SIP στο πεδίο ProxyAddresses](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) στην τοπική υπηρεσία καταλόγου Active Directory είναι μοναδική και η μορφή ταιριάζει sip:**Όνομα** χρήστη του χρήστη από το κέντρο διαχείρισης [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="9c6ee-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="9c6ee-112">Εάν σκοπεύετε να διατηρήσετε μια ανάπτυξη του Skype για επιχειρήσεις Server και να έχετε χρήστες εσωτερικής εγκατάστασης και Online: ακολουθήστε την "Ρύθμιση υβριδικής λειτουργίας με το Teams και το **Skype για επιχειρήσεις Online"** στον Πίνακα Ελέγχου του Skype για επιχειρήσεις Server και μετακινήστε τους χρήστες online.</span><span class="sxs-lookup"><span data-stu-id="9c6ee-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
