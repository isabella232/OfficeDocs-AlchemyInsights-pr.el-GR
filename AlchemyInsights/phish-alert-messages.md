---
title: Τα μηνύματα ειδοποίησης ηλεκτρονικού ταχυδρομείου 2491 από την πολιτική 'Override Phish παράδοση λόγω μισθωτών ή χρήστη'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391292"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="3f582-102">Μηνύματα ειδοποίησης ηλεκτρονικού ταχυδρομείου από την πολιτική 'Override Phish παράδοση λόγω μισθωτών ή χρήστη'</span><span class="sxs-lookup"><span data-stu-id="3f582-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="3f582-103">Μια προεπιλεγμένη πολιτική ειδοποίησης που ονομάζεται "Phish Delivered λόγω μισθωτών ή χρήστη παράκαμψη" έχει εφαρμόσει σε ενοίκους με άδειες χρήσης του Office 365 ATP P1 και P2.</span><span class="sxs-lookup"><span data-stu-id="3f582-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="3f582-104">Εάν λάβατε αυτήν την προειδοποίηση, ακολουθούν τα βήματα για να εξετάσετε:</span><span class="sxs-lookup"><span data-stu-id="3f582-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="3f582-105">Από το μήνυμα ειδοποίησης, κάντε κλικ στην επιλογή **Προβολή ειδοποίησης** για να μεταβείτε στη σελίδα **ειδοποιήσεων** της & ασφαλείας κέντρο συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="3f582-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="3f582-106">Επιλέξτε την ειδοποίηση για να δείτε την επιλογή **Προβολή λίστας μηνυμάτων** ή **Προβολή μηνυμάτων στην Εξερεύνηση**.</span><span class="sxs-lookup"><span data-stu-id="3f582-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="3f582-107">Και οι δύο αυτές τις επιλογές σας δίνουν τις λεπτομέρειες του μηνύματος, η οποία περιλαμβάνει το αναγνωριστικό μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="3f582-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="3f582-108">Σημειώστε ότι η σύνδεση απειλή Explorer θα φιλτράρει αυτόματα τα μηνύματα που ταιριάζουν με τα κριτήρια προειδοποιήσεων.</span><span class="sxs-lookup"><span data-stu-id="3f582-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="3f582-109">Ίσως χρειαστεί να ρυθμίσετε το φίλτρο ημερομηνίας στην Εξερεύνηση απειλή.</span><span class="sxs-lookup"><span data-stu-id="3f582-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="3f582-110">Το μήνυμα ηλεκτρονικού "ψαρέματος" παραδόθηκε εξαιτίας ενός έχει ρυθμιστεί με μη αυτόματο τρόπο παράκαμψης:</span><span class="sxs-lookup"><span data-stu-id="3f582-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="3f582-111">Ένα επιτρεπόμενο αποστολέα ή τον τομέα που καθορίζεται από το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="3f582-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="3f582-112">Ένα επιτρεπόμενων αποστολέα ή τομέα που έχουν οριστεί από το διαχειριστή σε μια πολιτική κατά της ανεπιθύμητης αλληλογραφίας.</span><span class="sxs-lookup"><span data-stu-id="3f582-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="3f582-113">Επιτρεπόμενο διεύθυνσης IP σε μια πολιτική φίλτρο σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="3f582-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="3f582-114">Μια ροή κανόνα αλληλογραφίας (γνωστό και ως έναν κανόνα μεταφοράς) που έχει ρυθμιστεί για να επιτρέψετε μηνύματα στο.</span><span class="sxs-lookup"><span data-stu-id="3f582-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="3f582-115">Εάν πιστεύετε ότι το μήνυμα έχει επισημανθεί εσφαλμένα ως ψαρεύουν, χρησιμοποιήστε το Outlook [προσθέτου μήνυμα αναφοράς](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) για να υποβάλλει δείγματα μήνυμα στη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3f582-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
