---
title: Προσθήκη καθολικής εταιρικής υπογραφής ή αποποίησης ευθυνών για όλους τους χρήστες
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: cbd92f9c4a78139eac4e3672dd0632b173472757
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50508589"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="da09c-102">Προσθήκη καθολικής εταιρικής υπογραφής ή αποποίησης ευθυνών για όλους τους χρήστες</span><span class="sxs-lookup"><span data-stu-id="da09c-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="da09c-103">Συμβουλή: Μια υπογραφή σε επίπεδο οργανισμού ονομάζεται επίσης αποποίηση ευθυνών, ανεξάρτητα από το τι περιλαμβάνει.</span><span class="sxs-lookup"><span data-stu-id="da09c-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="da09c-104">Στο κέντρο διαχείρισης, επιλέξτε **"Κέντρα διαχείρισης**  >  **Exchange".**</span><span class="sxs-lookup"><span data-stu-id="da09c-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="da09c-105">Στην περιοχή "Ροή αλληλογραφίας", επιλέξτε **"Κανόνες".**</span><span class="sxs-lookup"><span data-stu-id="da09c-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="da09c-106">Κάντε κλικ στο **+** εικονίδιο (Προσθήκη) και επιλέξτε **"Εφαρμογή αποποίησης ευθυνών".**</span><span class="sxs-lookup"><span data-stu-id="da09c-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="da09c-107">Δώστε ένα όνομα στον κανόνα.</span><span class="sxs-lookup"><span data-stu-id="da09c-107">Give the rule a name.</span></span>
5. <span data-ttu-id="da09c-108">Στην περιοχή "Εφαρμογή αυτού του κανόνα", επιλέξτε **"Εφαρμογή σε όλα τα μηνύματα".**</span><span class="sxs-lookup"><span data-stu-id="da09c-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="da09c-109">Στην περιοχή "Κάντε τα εξής", αφήστε επιλεγμένη **την επιλογή "Προσάρτηση αποποίησης** ευθυνών".</span><span class="sxs-lookup"><span data-stu-id="da09c-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="da09c-110">Κάντε κλικ **στην επιλογή "Εισαγωγή κειμένου"** και πληκτρολογήστε την αποποίηση ευθυνών.</span><span class="sxs-lookup"><span data-stu-id="da09c-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="da09c-111">Κάντε κλικ **σε μία επιλογή,** επιλέξτε **"Αναδίπλωση** ως εναλλακτική επιλογή" και, στη συνέχεια, κάντε κλικ στο **κουμπί OK.**</span><span class="sxs-lookup"><span data-stu-id="da09c-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="da09c-112">Αυτό σημαίνει ότι εάν η αποποίηση ευθυνών δεν μπορεί να προστεθεί λόγω κρυπτογράφησης ή άλλης ρύθμισης αλληλογραφίας, θα αναδιπλωθεί σε ένα φάκελο μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="da09c-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="da09c-113">Αφήστε τον **έλεγχο σε αυτόν τον** κανόνα με επιλεγμένο επίπεδο σοβαρότητας.</span><span class="sxs-lookup"><span data-stu-id="da09c-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="da09c-114">Στη συνέχεια, επιλέξτε "Χαμηλή", "Μεσαία" ή "Υψηλή" για να τη χρησιμοποιηθείτε στο αρχείο καταγραφής μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="da09c-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="da09c-115">Επιλέξτε **"Επιβολή",** για να ενεργοποιήσετε αμέσως την αποποίηση ευθυνών, εκτός αν θέλετε να τη δοκιμάσετε πρώτα.</span><span class="sxs-lookup"><span data-stu-id="da09c-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="da09c-116">Επιλέξτε **"Περισσότερες επιλογές"** για να συμπεριλάβετε πρόσθετες συνθήκες ή εξαιρέσεις.</span><span class="sxs-lookup"><span data-stu-id="da09c-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="da09c-117">Όταν τελειώσετε, κάντε κλικ στην επιλογή **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="da09c-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="da09c-118">Χρειάζεστε περισσότερη βοήθεια;</span><span class="sxs-lookup"><span data-stu-id="da09c-118">Need more help?</span></span> [<span data-ttu-id="da09c-119">Παρακολουθήστε ένα βίντεο σχετικά με τη δημιουργία αποποίησης ευθυνών ή διαβάστε ολόκληρο το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="da09c-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)