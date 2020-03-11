---
title: Είσοδος στα Windows 10 χωρίς χρήση κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588281"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="5437c-102">Είσοδος στα Windows 10 χωρίς χρήση κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="5437c-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="5437c-103">Για να αποφύγετε να πληκτρολογήσετε έναν κωδικό πρόσβασης κατά την εκκίνηση των Windows, συνιστούμε να χρησιμοποιήσετε μία από τις επιλογές εισόδου ασφαλούς εισόδου του Windows Hello, όπως pin, αναγνώριση προσώπου ή δακτυλικό αποτύπωμα, εάν υπάρχει.</span><span class="sxs-lookup"><span data-stu-id="5437c-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="5437c-104">Αν θέλετε πραγματικά να απενεργοποιήσετε την ασφαλή είσοδο, ανατρέξτε στις οδηγίες "Αυτόματη είσοδος στα Windows 10" παρακάτω.</span><span class="sxs-lookup"><span data-stu-id="5437c-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="5437c-105">**Ασφαλείς εναλλακτικές λύσεις του Windows Hello στον κωδικό πρόσβασης λογαριασμού**</span><span class="sxs-lookup"><span data-stu-id="5437c-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="5437c-106">Μεταβείτε στις **επιλογές "Ρυθμίσεις > λογαριασμοί > είσοδο"** (ή κάντε κλικ [εδώ).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="5437c-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="5437c-107">Θα εμφανίζονται οι διαθέσιμες επιλογές εισόδου.</span><span class="sxs-lookup"><span data-stu-id="5437c-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="5437c-108">Για παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="5437c-108">For example:</span></span>

![Επιλογές εισόδου.](media/sign-in-options.png)

<span data-ttu-id="5437c-110">Κάντε κλικ ή πατήστε μία από τις επιλογές για να ρυθμίσετε τις παραμέτρους της.</span><span class="sxs-lookup"><span data-stu-id="5437c-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="5437c-111">Την επόμενη φορά που θα ξεκινήσετε ή να ξεκλειδώσετε τα Windows, θα μπορείτε να χρησιμοποιήσετε τη νέα επιλογή αντί για έναν κωδικό πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="5437c-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="5437c-112">**Αυτόματη είσοδος στα Windows 10**</span><span class="sxs-lookup"><span data-stu-id="5437c-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="5437c-113">**Σημείωση**: Η αυτόματη είσοδος είναι βολική, αλλά εισάγει έναν κίνδυνο ασφαλείας, ειδικά αν ο υπολογιστής σας είναι προσβάσιμος από πολλά άτομα.</span><span class="sxs-lookup"><span data-stu-id="5437c-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="5437c-114">Κάντε κλικ ή πατήστε το κουμπί **Έναρξη** στη γραμμή εργασιών.</span><span class="sxs-lookup"><span data-stu-id="5437c-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="5437c-115">Πληκτρολογήστε **netplwiz** και πατήστε το πλήκτρο Enter για να ανοίξετε το παράθυρο Λογαριασμοί χρηστών.</span><span class="sxs-lookup"><span data-stu-id="5437c-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="5437c-116">Στην περιοχή **Λογαριασμοί χρηστών**, κάντε κλικ στο λογαριασμό στον οποίο θέλετε να εισέλθετε αυτόματα κατά την εκκίνηση των Windows.</span><span class="sxs-lookup"><span data-stu-id="5437c-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="5437c-117">Καταργήστε την επιλογή του πλαισίου ελέγχου "Οι χρήστες πρέπει να εισαγάγουν ένα όνομα χρήστη και έναν κωδικό πρόσβασης για να χρησιμοποιήσουν αυτόν τον υπολογιστή".</span><span class="sxs-lookup"><span data-stu-id="5437c-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Οι χρήστες πρέπει να εισαγάγουν μια επιλογή ονόματος χρήστη και κωδικού πρόσβασης.](media/users-must-enter-username.png)

5. <span data-ttu-id="5437c-119">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="5437c-119">Click **OK**.</span></span> <span data-ttu-id="5437c-120">Θα σας ζητηθεί να εισαγάγετε και να επιβεβαιώσετε τον κωδικό πρόσβασης για το λογαριασμό που επιλέξατε.</span><span class="sxs-lookup"><span data-stu-id="5437c-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="5437c-121">Κάντε κλικ στο **κουμπί OK** για να ολοκληρώσετε.</span><span class="sxs-lookup"><span data-stu-id="5437c-121">Click **OK** to finish.</span></span> <span data-ttu-id="5437c-122">Την επόμενη φορά που θα ξεκινήσουν τα Windows 10, θα εισέλθετε αυτόματα στον λογαριασμό που επιλέξατε.</span><span class="sxs-lookup"><span data-stu-id="5437c-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
