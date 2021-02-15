---
title: Αποκλεισμός υπογραφών ηλεκτρονικού ταχυδρομείου που έχουν γίνει από τον χρήστη
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
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243423"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="7afc5-102">Αποκλεισμός υπογραφών ηλεκτρονικού ταχυδρομείου που έχουν γίνει από τον χρήστη</span><span class="sxs-lookup"><span data-stu-id="7afc5-102">Block user-made email signatures</span></span>

<span data-ttu-id="7afc5-103">Η παρακάτω λύση ισχύει μόνο για τις υπογραφές ηλεκτρονικού ταχυδρομείου που δημιουργούνται στο Outlook στο web.</span><span class="sxs-lookup"><span data-stu-id="7afc5-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="7afc5-104">Μπορείτε να αποκλείσετε υπογραφές στην εφαρμογή Outlook μόνο εάν έχετε Exchange Server εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="7afc5-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="7afc5-105">Στο κέντρο διαχείρισης, επιλέξτε **"Κέντρα διαχείρισης",**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="7afc5-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="7afc5-106">Κάντε κλικ **στις**  >  **πολιτικές του Outlook Web App για δικαιώματα.**</span><span class="sxs-lookup"><span data-stu-id="7afc5-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="7afc5-107">Επιλέξτε την πολιτική και, στη συνέχεια, κάντε κλικ στο εικονίδιο μολυβιού για να την επεξεργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="7afc5-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="7afc5-108">Κάντε κλικ **στις δυνατότητες**  >  **"Περισσότερες επιλογές".**</span><span class="sxs-lookup"><span data-stu-id="7afc5-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="7afc5-109">Στην περιοχή **"Εμπειρία χρήστη",** καταργήστε την επιλογή του πλαισίου **ελέγχου "Υπογραφή ηλεκτρονικού ταχυδρομείου"** και, στη συνέχεια, κάντε κλικ στην **επιλογή "Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="7afc5-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="7afc5-110">**Σημαντικό:** Εάν μια υπογραφή προστέθηκε πριν από την απαλοιφή αυτού του πλαισίου ελέγχου, ο χρήστης θα εξακολουθεί να μπορεί να τη χρησιμοποιήσει.</span><span class="sxs-lookup"><span data-stu-id="7afc5-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="7afc5-111">Ζητήστε του να το καταργήσει.</span><span class="sxs-lookup"><span data-stu-id="7afc5-111">Ask them to remove it.</span></span>
