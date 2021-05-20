---
title: 2491 Μηνύματα ηλεκτρονικού ταχυδρομείου ειδοποίησης από την πολιτική "Παράδοση ηλεκτρονικού "ψαρέματος" λόγω αντικατάστασης μισθωτή ή χρήστη
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544578"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="deb9b-102">Ειδοποίηση μηνυμάτων ηλεκτρονικού ταχυδρομείου από την πολιτική "Ηλεκτρονικό "Ψάρεμα" λόγω αντικατάστασης μισθωτή ή χρήστη</span><span class="sxs-lookup"><span data-stu-id="deb9b-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="deb9b-103">Μια προεπιλεγμένη πολιτική ειδοποίησης με το όνομα "Ηλεκτρονικό "Ψάρεμα" παραδόθηκε λόγω αντικατάστασης μισθωτή ή χρήστη" έχει παραδοθεί στους μισθωτές με τον Microsoft Defender για άδειες χρήσης Office 365 P1 και P2.</span><span class="sxs-lookup"><span data-stu-id="deb9b-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="deb9b-104">Εάν λάβατε αυτή την ειδοποίηση, ακολουθούν τα βήματα που πρέπει να διερευνήσετε:</span><span class="sxs-lookup"><span data-stu-id="deb9b-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="deb9b-105">Από το μήνυμα ειδοποίησης, κάντε  **κλικ στην επιλογή** "Προβολή ειδοποίησης" για να μεταβείτε στη σελίδα "Ειδοποιήσεις" στο Κέντρο & συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="deb9b-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="deb9b-106">Επιλέξτε την ειδοποίηση για να δείτε την επιλογή "Προβολή **λίστας μηνυμάτων" ή** **"Προβολή μηνυμάτων" στην Εξερεύνηση.**</span><span class="sxs-lookup"><span data-stu-id="deb9b-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="deb9b-107">Και οι δύο αυτές επιλογές σας λαμβάνουν υπόψη τις λεπτομέρειες του μηνύματος, το οποίο περιλαμβάνει το αναγνωριστικό μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="deb9b-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="deb9b-108">Σημειώστε ότι η σύνδεση "Εξερεύνηση απειλών" θα φιλτράρει αυτόματα τα μηνύματα που πληρούν τα κριτήρια ειδοποίησης.</span><span class="sxs-lookup"><span data-stu-id="deb9b-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="deb9b-109">Ίσως χρειαστεί να προσαρμόσετε το φίλτρο ημερομηνίας στην Εξερεύνηση απειλών.</span><span class="sxs-lookup"><span data-stu-id="deb9b-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="deb9b-110">Το μήνυμα ηλεκτρονικού "ψαρέματος" παραδόθηκε λόγω παράκαμψης με μη αυτόματο τρόπο:</span><span class="sxs-lookup"><span data-stu-id="deb9b-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="deb9b-111">Ένας επιτρεπόμενος αποστολέας ή τομέας που έχει οριστεί από το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="deb9b-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="deb9b-112">Ένας επιτρεπόμενος αποστολέας ή τομέας που έχει οριστεί από το διαχειριστή σε μια πολιτική καταπολέμησης της ανεπιθύμητης αλληλογραφίας.</span><span class="sxs-lookup"><span data-stu-id="deb9b-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="deb9b-113">Μια επιτρεπόμενη διεύθυνση IP σε μια πολιτική φίλτρου σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="deb9b-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="deb9b-114">Ένας κανόνας ροής αλληλογραφίας (γνωστός και ως κανόνας μεταφοράς) που έχει ρυθμιστεί ώστε να επιτρέπει την αποστολή μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="deb9b-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="deb9b-115">Εάν πιστεύετε ότι το μήνυμα έχει επισημανθεί εσφαλμένα ως ηλεκτρονικό "ψάρεμα", χρησιμοποιήστε το πρόσθετο Outlook "Αναφορά [μηνύματος"](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) για να υποβάλετε δείγματα μηνυμάτων στη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="deb9b-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
