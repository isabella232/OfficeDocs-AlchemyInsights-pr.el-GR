---
title: Προηγμένες έννοιες ελέγχου ταυτότητας που ισχύουν για το Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573396"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="037c1-102">Προηγμένες έννοιες ελέγχου ταυτότητας που ισχύουν για το Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="037c1-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="037c1-103">Ακολουθούν οι προηγμένες έννοιες ελέγχου ταυτότητας που ισχύουν για το Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="037c1-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="037c1-104">**Ενεργός έλεγχος ταυτότητας**</span><span class="sxs-lookup"><span data-stu-id="037c1-104">**Proactive Authentication**</span></span>

<span data-ttu-id="037c1-105">Όταν ενεργοποιείτε την πολιτική [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , το Microsoft Edge θα προσπαθήσει να επικυρώνει προληπτικά τους χρήστες που έχουν συνδεθεί μέσω των υπηρεσιών της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="037c1-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="037c1-106">Σε τακτά χρονικά διαστήματα, θα χρησιμοποιήσει μια ηλεκτρονική υπηρεσία για να ελέγχει για μια ενημερωμένη δήλωση που περιέχει τις ρυθμίσεις παραμέτρων που διέπουν τον προορατικό έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="037c1-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="037c1-107">Πλεονεκτήματα: ο ενεργός έλεγχος ταυτότητας επιτρέπει τον έλεγχο ταυτότητας σε βασικές υπηρεσίες, όπως η σελίδα "νέα καρτέλα" του Office.</span><span class="sxs-lookup"><span data-stu-id="037c1-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="037c1-108">Επίσης, εάν το Bing χρησιμοποιείται ως μηχανή αναζήτησης, ο προληπτική έλεγχος ταυτότητας βελτιώνει τις επιδόσεις της γραμμής διευθύνσεων και συμβάλλει στη δημιουργία προσαρμοσμένων αποτελεσμάτων αναζήτησης στις ανάγκες της επιχείρησής σας.</span><span class="sxs-lookup"><span data-stu-id="037c1-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="037c1-109">**Windows Hello CredUI για έλεγχο ταυτότητας NTLM**</span><span class="sxs-lookup"><span data-stu-id="037c1-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="037c1-110">Εάν η καθολική σύνδεση (SSO) δεν είναι διαθέσιμη όταν μια τοποθεσία Web επιχειρεί να πραγματοποιήσει είσοδο στο χρήστη μέσω του μηχανισμού NTLM ή διαπραγμάτευσης, αυτή η δυνατότητα θα επιτρέψει στο χρήστη να κάνει κοινή χρήση των διαπιστευτηρίων του λειτουργικού συστήματος με την τοποθεσία Web και να ικανοποιήσει την πρόκληση ελέγχου ταυτότητας χρησιμοποιώντας το περιβάλλον εργασίας χρήστη του Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="037c1-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="037c1-111">Αυτή η ροή εισόδου θα εμφανίζεται μόνο στα Windows 10 και μόνο για τους χρήστες που δεν έχουν SSO κατά τη διάρκεια ενός NTLM ή μιας πρόκλησης διαπραγμάτευσης.</span><span class="sxs-lookup"><span data-stu-id="037c1-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="037c1-112">**Χρήση αποθηκευμένων κωδικών πρόσβασης για αυτόματη είσοδο**</span><span class="sxs-lookup"><span data-stu-id="037c1-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="037c1-113">Οι χρήστες που αποθηκεύουν κωδικούς πρόσβασης στο Microsoft Edge μπορούν να ενεργοποιήσουν την αυτόματη σύνδεση σε τοποθεσίες Web όπου έχουν αποθηκεύσει διαπιστευτήρια.</span><span class="sxs-lookup"><span data-stu-id="037c1-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="037c1-114">Οι χρήστες μπορούν να ενεργοποιούν ή να απενεργοποιούν αυτή τη δυνατότητα στο edge://settings/passwords και μπορείτε να τις ρυθμίσετε στις πολιτικές [διαχείρισης κωδικών πρόσβασης](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="037c1-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
