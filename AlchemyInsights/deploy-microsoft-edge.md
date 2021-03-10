---
title: Ανάπτυξη του Microsoft Edge
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
- "9139"
- "9005291"
ms.openlocfilehash: ad2c42ad77cd4a4606365bc616547846ae3c2c65
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693572"
---
# <a name="deploy-microsoft-edge"></a><span data-ttu-id="ece55-102">Ανάπτυξη του Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ece55-102">Deploy Microsoft Edge</span></span>

<span data-ttu-id="ece55-103">Αφού έχετε καθορίσει τις πολιτικές σας και έχετε ολοκληρώσει τον αρχικό έλεγχο συμβατότητας εφαρμογών, είστε έτοιμοι να αναπτύξετε την πιλοτική ομάδα σας.</span><span class="sxs-lookup"><span data-stu-id="ece55-103">After you've defined your policies and have finished your initial app compatibility testing, you're ready to deploy to your pilot group.</span></span> <span data-ttu-id="ece55-104">Η ανάπτυξη σε μια πιλοτική ομάδα σάς επιτρέπει να λάβετε σχόλια και να διορθώσετε προβλήματα πριν από την ανάπτυξη του Microsoft Edge σε ολόκληρο τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="ece55-104">Deploying to a pilot group lets you get feedback and fix issues before Microsoft Edge is rolled out to your entire organization.</span></span>

<span data-ttu-id="ece55-105">Διατίθενται τα ακόλουθα εργαλεία για την ανάπτυξη του Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="ece55-105">The following tools are available to deploy Microsoft Edge:</span></span>

- <span data-ttu-id="ece55-106">[Microsoft Intune για Windows ή](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge) [Microsoft Intune για macOS](https://docs.microsoft.com/mem/intune/apps/apps-edge-macos)</span><span class="sxs-lookup"><span data-stu-id="ece55-106">[Microsoft Intune for Windows](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge) or [Microsoft Intune for macOS](https://docs.microsoft.com/mem/intune/apps/apps-edge-macos)</span></span>
- [<span data-ttu-id="ece55-107">Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="ece55-107">Configuration Manager</span></span>](https://docs.microsoft.com/DeployEdge/deploy-edge-with-configuration-manager)
- <span data-ttu-id="ece55-108">Ένα άλλο εργαλείο που χρησιμοποιεί [το αρχείο MSI για τον Microsoft Edge](https://www.microsoft.com/edge/business/download)</span><span class="sxs-lookup"><span data-stu-id="ece55-108">Another tool using the [MSI file for Microsoft Edge](https://www.microsoft.com/edge/business/download)</span></span>

<span data-ttu-id="ece55-109">**Επικύρωση της ανάπτυξής σας**</span><span class="sxs-lookup"><span data-stu-id="ece55-109">**Validate your deployment**</span></span>

<span data-ttu-id="ece55-110">Μετά την ανάπτυξη της πιλοτικής λύσης σας, καταγράψτε τα σχόλια των χρηστών.</span><span class="sxs-lookup"><span data-stu-id="ece55-110">After you deploy your pilot, capture feedback from users.</span></span> <span data-ttu-id="ece55-111">Λάβετε υπόψη σας τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ece55-111">Consider the following:</span></span>
- <span data-ttu-id="ece55-112">**Συμβατότητα:** Προσδιορίστε τις τοποθεσίες που ανήκουν στη λίστα εταιρικών τοποθεσιών που δεν έχουν προσδιοριστεί κατά τον εντοπισμό της τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="ece55-112">**Compatibility**: Identify sites that belong on the Enterprise Site List that weren't identified during site discovery.</span></span>
- <span data-ttu-id="ece55-113">**Ρύθμιση παραμέτρων** πολιτικής: Βεβαιωθείτε ότι οι χρήστες μπορούν να χρησιμοποιούν βασικές δυνατότητες και να κάνουν την εργασία τους ακολουθώντας τις οδηγίες ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="ece55-113">**Policy configuration**: Ensure that users can use key features and do their work while following security guidelines.</span></span>
- <span data-ttu-id="ece55-114">**Ευκολία στη χρήση και νέες δυνατότητες:** Προσδιορίστε τους τομείς όπου πρέπει να αναπτυχθεί και να παραδοθεί η εκπαίδευση με βάση τις ερωτήσεις των χρηστών.</span><span class="sxs-lookup"><span data-stu-id="ece55-114">**Ease of use and new features**: Identify any areas where training should be developed and delivered based on user questions.</span></span>

<span data-ttu-id="ece55-115">**Ευρεία ανάπτυξη του Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="ece55-115">**Broad deployment of Microsoft Edge**</span></span>

<span data-ttu-id="ece55-116">Αφού αναπτύξετε το πιλοτικό και ενημερωμένο σχέδιο ανάπτυξης με τα μαθήματα που έχετε μάθει, είστε έτοιμοι να κάνετε μια πλήρη ανάπτυξη του Microsoft Edge σε όλους τους χρήστες σας.</span><span class="sxs-lookup"><span data-stu-id="ece55-116">Once you've deployed the pilot and updated your deployment plan with lessons learnt, you're ready to do a full deployment of Microsoft Edge to all your users.</span></span> <span data-ttu-id="ece55-117">Συγχαρητήρια!!</span><span class="sxs-lookup"><span data-stu-id="ece55-117">Congratulations!</span></span>

