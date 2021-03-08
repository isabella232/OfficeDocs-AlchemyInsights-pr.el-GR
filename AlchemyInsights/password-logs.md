---
title: Αρχεία καταγραφής κωδικών πρόσβασης
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525138"
---
# <a name="password-logs"></a><span data-ttu-id="5ee97-102">Αρχεία καταγραφής κωδικών πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="5ee97-102">Password logs</span></span>

<span data-ttu-id="5ee97-103">**Έχω προβλήματα κατά την πρόσβαση σε αρχεία καταγραφής ελέγχου επαναφοράς κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="5ee97-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="5ee97-104">Για την αντιμετώπιση προβλημάτων σχετικά με την πρόσβαση σε αρχεία καταγραφής ελέγχου επαναφοράς κωδικού πρόσβασης, εκτελέστε το παρακάτω βήμα:</span><span class="sxs-lookup"><span data-stu-id="5ee97-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="5ee97-105">Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι για την προβολή των αρχείων καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="5ee97-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="5ee97-106">Μόνο οι παρακάτω ρόλοι είναι εξουσιοδοτημένοι:</span><span class="sxs-lookup"><span data-stu-id="5ee97-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="5ee97-107">Καθολικός διαχειριστής</span><span class="sxs-lookup"><span data-stu-id="5ee97-107">Global administrator</span></span>
 - <span data-ttu-id="5ee97-108">Διαχειριστής ασφαλείας</span><span class="sxs-lookup"><span data-stu-id="5ee97-108">Security administrator</span></span>
 - <span data-ttu-id="5ee97-109">Πρόγραμμα ανάγνωσης ασφαλείας</span><span class="sxs-lookup"><span data-stu-id="5ee97-109">Security reader</span></span>

<span data-ttu-id="5ee97-110">**Θέλω να δω όλα τα συμβάντα ελέγχου επαναφοράς κωδικού πρόσβασης από τη στιγμή που αναπτύξαμε αρχικά**</span><span class="sxs-lookup"><span data-stu-id="5ee97-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="5ee97-111">Έως και 120.000 συμβάντα επαναφοράς/καταχώρησης κωδικού πρόσβασης αποθηκεύονται στις αναφορές των τελευταίων 30 ημερών.</span><span class="sxs-lookup"><span data-stu-id="5ee97-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="5ee97-112">Αυτό το μέγιστο όριο ισχύει για το περιβάλλον εργασίας χρήστη κατά τη λήψη του CSV.</span><span class="sxs-lookup"><span data-stu-id="5ee97-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="5ee97-113">1 εκατομμύριο συμβάντα είναι διαθέσιμες μέσω του PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5ee97-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="5ee97-114">Για περισσότερες πληροφορίες, ανατρέξτε στις παρακάτω συνδέσεις:</span><span class="sxs-lookup"><span data-stu-id="5ee97-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="5ee97-115">Συμβάντα επαναφοράς κωδικού πρόσβασης από το χρήστη από το API αναφορών και συμβάντων του Azure AD</span><span class="sxs-lookup"><span data-stu-id="5ee97-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5ee97-116">Πώς μπορείτε να κάνετε λήψη συμβάντων καταχώρησης επαναφοράς κωδικού πρόσβασης γρήγορα με το PowerShell</span><span class="sxs-lookup"><span data-stu-id="5ee97-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="5ee97-117">**Θέλω να κατανοήσω περισσότερα σχετικά με τις δυνατότητες αναφοράς επαναφοράς κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="5ee97-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="5ee97-118">Ελέγξτε ποιος καταχωρεί ή επαναφέρει κωδικούς πρόσβασης με αρχεία καταγραφής ελέγχου επαναφοράς κωδικού πρόσβασης του Azure AD στην πύλη Azure, στην περιοχή Χρήστες **και ομάδες.**</span><span class="sxs-lookup"><span data-stu-id="5ee97-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="5ee97-119">Για περισσότερες πληροφορίες, ανατρέξτε στις παρακάτω συνδέσεις:</span><span class="sxs-lookup"><span data-stu-id="5ee97-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="5ee97-120">Επισκόπηση αναφορών επαναφοράς κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="5ee97-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5ee97-121">Πώς μπορείτε να προβάλετε αναφορές επαναφοράς κωδικού πρόσβασης στην πύλη Azure</span><span class="sxs-lookup"><span data-stu-id="5ee97-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5ee97-122">Συμβάντα επαναφοράς κωδικού πρόσβασης από το χρήστη από το API αναφορών και συμβάντων του Azure AD</span><span class="sxs-lookup"><span data-stu-id="5ee97-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5ee97-123">Πώς μπορείτε να κάνετε λήψη συμβάντων καταχώρησης επαναφοράς κωδικού πρόσβασης γρήγορα με το PowerShell</span><span class="sxs-lookup"><span data-stu-id="5ee97-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


