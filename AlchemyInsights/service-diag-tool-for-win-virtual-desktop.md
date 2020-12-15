---
title: Εργαλείο διαγνωστικών υπηρεσιών για την εικονική επιφάνεια εργασίας των Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678619"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="c35fd-102">Εργαλείο διαγνωστικών υπηρεσιών για την εικονική επιφάνεια εργασίας των Windows</span><span class="sxs-lookup"><span data-stu-id="c35fd-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="c35fd-103">Το Windows Virtual Desktop (WVD) προσφέρει ένα διαγνωστικό εργαλείο που επιτρέπει στους διαχειριστές να εντοπίζουν σφάλματα μέσω μιας μεμονωμένης διασύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="c35fd-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="c35fd-104">Αυτό το εργαλείο καταγράφει πληροφορίες που σχετίζονται με τα διαγνωστικά κάθε φορά που χρησιμοποιείται το WVD από κάποιον που έχει εκχωρήσει ένα ρόλο WVD.</span><span class="sxs-lookup"><span data-stu-id="c35fd-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="c35fd-105">Κάθε αρχείο καταγραφής περιέχει πληροφορίες σχετικά με το ρόλο του WVD που εμπλέκεται στη δραστηριότητα, τα μηνύματα σφάλματος που εμφανίζονται κατά τη διάρκεια της περιόδου λειτουργίας και τις πληροφορίες σχετικά με τον μισθωτή και το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="c35fd-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="c35fd-106">Η ανάλυση του αρχείου καταγραφής Azure μπορεί να ρυθμιστεί για την καταγραφή του αρχείου καταγραφής δραστηριοτήτων που δημιουργήθηκε από το εργαλείο διάγνωσης.</span><span class="sxs-lookup"><span data-stu-id="c35fd-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="c35fd-107">Αυτό μπορεί να γίνει ως εξής:</span><span class="sxs-lookup"><span data-stu-id="c35fd-107">Here's how:</span></span>

1. <span data-ttu-id="c35fd-108">Δημιουργήστε ένα χώρο εργασίας του αρχείου καταγραφής ανάλυσης με την [πύλη Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ή το [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="c35fd-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="c35fd-109">[Συνδέστε τους υπολογιστές με Windows στην οθόνη Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="c35fd-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="c35fd-110">Λήψη του ΑΝΑΓΝΩΡΙΣΤΙΚού χώρου εργασίας και του πρωτεύοντος κλειδιού του χώρου εργασίας σας.</span><span class="sxs-lookup"><span data-stu-id="c35fd-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="c35fd-111">Ο οδηγός εγκατάστασης χρειάζεται αυτές τις πληροφορίες για να ρυθμίσει σωστά τις παραμέτρους του παράγοντα και να εξασφαλίσει ότι μπορεί να επικοινωνεί με την οθόνη Azure.</span><span class="sxs-lookup"><span data-stu-id="c35fd-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="c35fd-112">[Σπρώξτε τα δεδομένα διαγνωστικών στο χώρο εργασίας σας](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="c35fd-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="c35fd-113">Μπορείτε να πιέσετε τα διαγνωστικά δεδομένα από τον μισθωτή του WVD στην ανάλυση καταγραφής για το χώρο εργασίας σας.</span><span class="sxs-lookup"><span data-stu-id="c35fd-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="c35fd-114">[Προσδιορίστε και Διαγνώστε προβλήματα](https://go.microsoft.com/fwlink/?linkid=2128338) που είναι εσωτερικά ή εξωτερικά σε σχέση με το WVD.</span><span class="sxs-lookup"><span data-stu-id="c35fd-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="c35fd-115">Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων του εργαλείου διαγνωστικών υπηρεσιών για το WVD, ανατρέξτε στο θέμα [χρήση της ανάλυσης καταγραφής για τη δυνατότητα διαγνωστικών](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="c35fd-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
