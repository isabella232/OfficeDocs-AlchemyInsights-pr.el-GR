---
title: Προσθήκη καθολικής εταιρικής υπογραφής ή αποποίησης ευθυνών για όλους τους χρήστες
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ab0d3fc80b41b9017a6917817270438644f770b8
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482804"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="c1066-102">Προσθήκη καθολικής εταιρικής υπογραφής ή αποποίησης ευθυνών για όλους τους χρήστες</span><span class="sxs-lookup"><span data-stu-id="c1066-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="c1066-103">Συμβουλή: Μια υπογραφή σε επίπεδο οργανισμού ονομάζεται επίσης αποποίηση ευθυνών, ανεξάρτητα από το τι περιλαμβάνει.</span><span class="sxs-lookup"><span data-stu-id="c1066-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="c1066-104">Στο κέντρο διαχείρισης, επιλέξτε **"Κέντρα διαχείρισης",**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="c1066-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="c1066-105">Στην περιοχή "Ροή αλληλογραφίας", επιλέξτε **"Κανόνες".**</span><span class="sxs-lookup"><span data-stu-id="c1066-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="c1066-106">Κάντε κλικ στο **+** εικονίδιο (Προσθήκη) και επιλέξτε **"Εφαρμογή αποποίησης ευθυνών".**</span><span class="sxs-lookup"><span data-stu-id="c1066-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="c1066-107">Δώστε ένα όνομα στον κανόνα.</span><span class="sxs-lookup"><span data-stu-id="c1066-107">Give the rule a name.</span></span>
5. <span data-ttu-id="c1066-108">Στην περιοχή "Εφαρμογή αυτού του κανόνα", επιλέξτε **"Εφαρμογή σε όλα τα μηνύματα".**</span><span class="sxs-lookup"><span data-stu-id="c1066-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="c1066-109">Στην περιοχή "Κάντε τα εξής", αφήστε επιλεγμένη **την επιλογή "Προσάρτηση αποποίησης** ευθυνών".</span><span class="sxs-lookup"><span data-stu-id="c1066-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="c1066-110">Κάντε κλικ **στην επιλογή "Εισαγωγή κειμένου"** και πληκτρολογήστε την αποποίηση ευθυνών.</span><span class="sxs-lookup"><span data-stu-id="c1066-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="c1066-111">Κάντε κλικ **σε μία επιλογή,** επιλέξτε **"Αναδίπλωση** ως εναλλακτική επιλογή" και, στη συνέχεια, κάντε κλικ στο **κουμπί OK.**</span><span class="sxs-lookup"><span data-stu-id="c1066-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="c1066-112">Αυτό σημαίνει ότι εάν η αποποίηση ευθυνών δεν μπορεί να προστεθεί λόγω κρυπτογράφησης ή άλλης ρύθμισης αλληλογραφίας, θα αναδιπλωθεί σε ένα φάκελο μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="c1066-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="c1066-113">Αφήστε τον **έλεγχο σε αυτόν τον** κανόνα με επιλεγμένο επίπεδο σοβαρότητας.</span><span class="sxs-lookup"><span data-stu-id="c1066-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="c1066-114">Στη συνέχεια, επιλέξτε "Χαμηλή", "Μεσαία" ή "Υψηλή" για να τη χρησιμοποιηθείτε στο αρχείο καταγραφής μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="c1066-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="c1066-115">Επιλέξτε **"Επιβολή"** για να ενεργοποιήσετε αμέσως την αποποίηση ευθυνών, εκτός αν θέλετε να την δοκιμάσετε πρώτα.</span><span class="sxs-lookup"><span data-stu-id="c1066-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="c1066-116">Επιλέξτε **"Περισσότερες επιλογές"** για να συμπεριλάβετε πρόσθετες συνθήκες ή εξαιρέσεις.</span><span class="sxs-lookup"><span data-stu-id="c1066-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="c1066-117">Όταν τελειώσετε, κάντε κλικ στην επιλογή **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="c1066-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="c1066-118">Χρειάζεστε περισσότερη βοήθεια;</span><span class="sxs-lookup"><span data-stu-id="c1066-118">Need more help?</span></span> [<span data-ttu-id="c1066-119">Παρακολουθήστε ένα βίντεο σχετικά με τη δημιουργία αποποίησης ευθυνών ή διαβάστε ολόκληρο το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="c1066-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)