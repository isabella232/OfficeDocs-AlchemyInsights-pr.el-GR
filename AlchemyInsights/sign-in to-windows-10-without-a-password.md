---
title: Είσοδος στα Windows 10 χωρίς τη χρήση κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719953"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="08e01-102">Είσοδος στα Windows 10 χωρίς τη χρήση κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="08e01-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="08e01-103">Για να αποφύγετε την πληκτρολόγηση κωδικού πρόσβασης κατά την εκκίνηση των Windows, συνιστάται να χρησιμοποιήσετε μία από τις επιλογές εισόδου ασφαλούς σύνδεσης του Windows Hello, όπως PIN, αναγνώριση προσώπου ή δακτυλικό αποτύπωμα, εάν υπάρχει.</span><span class="sxs-lookup"><span data-stu-id="08e01-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="08e01-104">Εάν θέλετε πραγματικά να απενεργοποιήσετε την ασφαλή είσοδο, ανατρέξτε στις οδηγίες "Αυτόματη είσοδος στα Windows 10" παρακάτω.</span><span class="sxs-lookup"><span data-stu-id="08e01-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="08e01-105">**Ασφαλείς εναλλακτικές λύσεις του Windows Hello για τον κωδικό πρόσβασης του λογαριασμού**</span><span class="sxs-lookup"><span data-stu-id="08e01-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="08e01-106">Μεταβείτε στις **ρυθμίσεις > λογαριασμών > επιλογών εισόδου** (ή κάντε κλικ [εδώ](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="08e01-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="08e01-107">Οι διαθέσιμες επιλογές εισόδου θα παρατίθενται.</span><span class="sxs-lookup"><span data-stu-id="08e01-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="08e01-108">Για παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="08e01-108">For example:</span></span>

![Επιλογές εισόδου.](media/sign-in-options.png)

<span data-ttu-id="08e01-110">Κάντε κλικ ή πατήστε μία από τις επιλογές για να τις ρυθμίσετε.</span><span class="sxs-lookup"><span data-stu-id="08e01-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="08e01-111">Την επόμενη φορά που θα ξεκινήσετε ή θα ξεκλειδώσετε τα Windows, θα μπορείτε να χρησιμοποιήσετε τη νέα επιλογή αντί για έναν κωδικό πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="08e01-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="08e01-112">**Αυτόματη είσοδος στα Windows 10**</span><span class="sxs-lookup"><span data-stu-id="08e01-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="08e01-113">**Σημείωση**: η αυτόματη είσοδος είναι εύκολη, αλλά εισάγει έναν κίνδυνο ασφαλείας, ειδικά εάν ο υπολογιστής σας είναι προσβάσιμος από πολλά άτομα.</span><span class="sxs-lookup"><span data-stu-id="08e01-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="08e01-114">Κάντε κλικ ή πατήστε το κουμπί **Έναρξη** στη γραμμή εργασιών.</span><span class="sxs-lookup"><span data-stu-id="08e01-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="08e01-115">Πληκτρολογήστε **netplwiz** και πατήστε το πλήκτρο ENTER για να ανοίξετε το παράθυρο Λογαριασμοί χρηστών.</span><span class="sxs-lookup"><span data-stu-id="08e01-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="08e01-116">Στους **λογαριασμούς χρηστών**, κάντε κλικ στο λογαριασμό στον οποίο θέλετε να εισέλθετε αυτόματα κατά την εκκίνηση των Windows.</span><span class="sxs-lookup"><span data-stu-id="08e01-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="08e01-117">Καταργήστε την επιλογή του πλαισίου ελέγχου "οι χρήστες πρέπει να εισαγάγουν ένα όνομα χρήστη και κωδικό πρόσβασης για να χρησιμοποιήσουν αυτόν τον υπολογιστή".</span><span class="sxs-lookup"><span data-stu-id="08e01-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Οι χρήστες πρέπει να εισαγάγουν μια επιλογή ονόματος χρήστη και κωδικού πρόσβασης.](media/users-must-enter-username.png)

5. <span data-ttu-id="08e01-119">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="08e01-119">Click **OK**.</span></span> <span data-ttu-id="08e01-120">Θα σας ζητηθεί να εισαγάγετε και να επιβεβαιώσετε τον κωδικό πρόσβασης για τον λογαριασμό που επιλέξατε.</span><span class="sxs-lookup"><span data-stu-id="08e01-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="08e01-121">Κάντε κλικ στο κουμπί **OK** για να ολοκληρώσετε.</span><span class="sxs-lookup"><span data-stu-id="08e01-121">Click **OK** to finish.</span></span> <span data-ttu-id="08e01-122">Την επόμενη φορά που θα ξεκινήσουν τα Windows 10, θα συνδεθεί αυτόματα στο λογαριασμό που επιλέξατε.</span><span class="sxs-lookup"><span data-stu-id="08e01-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
