---
title: Δοκιμή συμβατότητας εφαρμογών
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
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693659"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="034aa-102">Δοκιμή συμβατότητας εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="034aa-102">Do app compatibility testing</span></span>

<span data-ttu-id="034aa-103">Η συμβατότητα εφαρμογών για τον Microsoft Edge είναι εξαιρετικά υψηλή.</span><span class="sxs-lookup"><span data-stu-id="034aa-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="034aa-104">Στην πραγματικότητα, είναι τόσο υψηλή που η Microsoft παρέχει τις ακόλουθες υπόσχεις συμβατότητας:</span><span class="sxs-lookup"><span data-stu-id="034aa-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="034aa-105">Εάν λειτουργεί στον Microsoft Edge 45 και σε παλαιότερες εκδόσεις, θα λειτουργεί στον Microsoft Edge 77 και σε νεότερες εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="034aa-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="034aa-106">Εάν λειτουργεί στον Internet Explorer, θα λειτουργεί στον Microsoft Edge σε λειτουργία Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="034aa-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="034aa-107">Εάν λειτουργεί στο Google Chrome, θα λειτουργεί στον Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="034aa-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="034aa-108">Εάν έχετε μια εφαρμογή όπου δεν ανταποκριθούμε σε αυτήν την υπόσχεσή σας, τότε είμαστε πίσω από την υπόσχεσή σας να τη διορθώσουμε με [το Microsoft App Assure.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="034aa-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="034aa-109">Παρά αυτή την υπόσχεση, γνωρίζουμε ότι πολλοί οργανισμοί πρέπει να επικυρώσουν ορισμένες εφαρμογές για λόγους συμμόρφωσης ή διαχείρισης κινδύνων.</span><span class="sxs-lookup"><span data-stu-id="034aa-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="034aa-110">Παρόλο που αναμένουμε ότι αυτό είναι πολύ άμεσο, είναι σημαντικό να είστε οργανωμένοι και αυστηρόι στον έλεγχο εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="034aa-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="034aa-111">Υπάρχουν δύο τρόποι για να κάνετε έλεγχο συμβατότητας εφαρμογών:</span><span class="sxs-lookup"><span data-stu-id="034aa-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="034aa-112">**Δοκιμή εργαστηρίου:** Οι εφαρμογές ελέγχονται σε ένα καλά ελεγχόμενο περιβάλλον με συγκεκριμένες διαμορφώσεις.</span><span class="sxs-lookup"><span data-stu-id="034aa-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="034aa-113">**Πιλοτικές δοκιμές:** Οι εφαρμογές δοκιμάονται από περιορισμένο αριθμό χρηστών στο καθημερινό περιβάλλον εργασίας τους χρησιμοποιώντας τις δικές τους συσκευές.</span><span class="sxs-lookup"><span data-stu-id="034aa-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="034aa-114">Επιλέξτε τη μέθοδο που είναι πιο κατάλληλη για κάθε εφαρμογή και κάντε τις δοκιμές πριν από την κυκλοφορία σε ολόκληρο τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="034aa-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="034aa-115">Αφού διασφαλίσετε ότι οι εφαρμογές σας είναι συμβατές, είστε έτοιμοι να αναπτύξετε τον Microsoft Edge σε μια πιλοτική ομάδα.</span><span class="sxs-lookup"><span data-stu-id="034aa-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
