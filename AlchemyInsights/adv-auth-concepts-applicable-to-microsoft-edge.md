---
title: Έννοιες ελέγχου ταυτότητας για προχωρημένους που ισχύουν για τον Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398562"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="6349f-102">Έννοιες ελέγχου ταυτότητας για προχωρημένους που ισχύουν για τον Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6349f-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="6349f-103">Ακολουθούν οι έννοιες ελέγχου ταυτότητας για προχωρημένους που ισχύουν για τον Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="6349f-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="6349f-104">**Προληπτικός έλεγχος ταυτότητας**</span><span class="sxs-lookup"><span data-stu-id="6349f-104">**Proactive Authentication**</span></span>

<span data-ttu-id="6349f-105">Όταν ενεργοποιήσετε την πολιτική [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) ο Microsoft Edge θα προσπαθήσει να πραγματοποιήσει προληπτικό έλεγχο ταυτότητας των χρηστών που είναι συνδεδεμένοι μέσω των υπηρεσιών της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6349f-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="6349f-106">Σε τακτά χρονικά διαστήματα, θα χρησιμοποιεί μια ηλεκτρονική υπηρεσία για να ελέγχει για μια ενημερωμένη διακήρυξη που περιέχει τη ρύθμιση παραμέτρων που διέπει τον προληπτικό έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="6349f-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="6349f-107">Πλεονεκτήματα: Ο προληπτικός έλεγχος ταυτότητας επιτρέπει τον έλεγχο ταυτότητας σε βασικές υπηρεσίες, όπως η σελίδα "Νέα καρτέλα του Office".</span><span class="sxs-lookup"><span data-stu-id="6349f-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="6349f-108">Επίσης, εάν το Bing χρησιμοποιείται ως μηχανισμός αναζήτησης, ο προληπτικός έλεγχος ταυτότητας βελτιώνει τις επιδόσεις της γραμμής διευθύνσεων και συμβάλλει στη δημιουργία αποτελεσμάτων αναζήτησης προσαρμοσμένων στις ανάγκες της επιχείρησής σας.</span><span class="sxs-lookup"><span data-stu-id="6349f-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="6349f-109">**Windows Hello CredUI για έλεγχο ταυτότητας NTLM**</span><span class="sxs-lookup"><span data-stu-id="6349f-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="6349f-110">Εάν η μεμονωμένη σύνδεση (SSO) δεν είναι διαθέσιμη όταν μια τοποθεσία Web προσπαθεί να συνδεθεί στο χρήστη μέσω του μηχανισμού NTLM ή Negotiate, αυτή η δυνατότητα θα επιτρέψει στο χρήστη να κάνει κοινή χρήση των διαπιστευτηρίων λειτουργικού συστήματος με την τοποθεσία Web και να ικανοποιεί την πρόκληση ελέγχου ταυτότητας χρησιμοποιώντας το περιβάλλον εργασίας χρήστη Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="6349f-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="6349f-111">Αυτή η ροή είσοδου θα εμφανίζεται μόνο στα Windows 10 και μόνο για τους χρήστες που δεν επιτρέπουν SSO κατά τη διάρκεια ενός NTLM ή μιας πρόκλησης "Διαπραγματευτείτε".</span><span class="sxs-lookup"><span data-stu-id="6349f-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="6349f-112">**Χρήση αποθηκευμένων κωδικών πρόσβασης για αυτόματη είσοδο**</span><span class="sxs-lookup"><span data-stu-id="6349f-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="6349f-113">Οι χρήστες που αποθηκεύσουν κωδικούς πρόσβασης στον Microsoft Edge μπορούν να ενεργοποιήσουν την αυτόματη είσοδο σε τοποθεσίες Web όπου έχουν αποθηκεύσει διαπιστευτήρια.</span><span class="sxs-lookup"><span data-stu-id="6349f-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="6349f-114">Οι χρήστες μπορούν να ενεργοποιήσουν ή να απενεργοποιήσουν αυτήν τη δυνατότητα edge://settings/passwords και μπορείτε να τη ρυθμίσετε στις πολιτικές διαχείρισης [κωδικών](https://go.microsoft.com/fwlink/?linkid=2134622) πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="6349f-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
