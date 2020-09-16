---
title: μηνύματα ηλεκτρονικού ταχυδρομείου ειδοποίησης του 2491 από την πολιτική "Phish παραδόθηκε λόγω μισθωτού ή παράκαμψης χρήστη"
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728611"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="df8f6-102">Ειδοποίηση μηνυμάτων ηλεκτρονικού ταχυδρομείου από την πολιτική "Phish παραδόθηκε λόγω μισθωτής ή παράκαμψης χρήστη"</span><span class="sxs-lookup"><span data-stu-id="df8f6-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="df8f6-103">Μια προεπιλεγμένη πολιτική ειδοποίησης με το όνομα "Phish παραδόθηκε λόγω μισθωτού ή παράκαμψης χρήστη" έχει εκχωρηθεί σε μισθωτές με άδειες χρήσης του Office 365 ATP P1 και P2.</span><span class="sxs-lookup"><span data-stu-id="df8f6-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="df8f6-104">Εάν λάβατε αυτή την ειδοποίηση, εδώ θα βρείτε τα βήματα που πρέπει να εξετάσετε:</span><span class="sxs-lookup"><span data-stu-id="df8f6-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="df8f6-105">Από το μήνυμα ειδοποίησης, κάντε κλικ στην επιλογή **Προβολή ειδοποίησης** για να μεταβείτε στη σελίδα **ειδοποιήσεις** στο κέντρο συμμόρφωσης & ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="df8f6-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="df8f6-106">Επιλέξτε την ειδοποίηση για να δείτε την επιλογή για να **προβάλετε τη λίστα μηνυμάτων** ή να **προβάλετε μηνύματα στην Εξερεύνηση**.</span><span class="sxs-lookup"><span data-stu-id="df8f6-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="df8f6-107">Και οι δύο αυτές επιλογές σας μεταλαμβάνουν στις λεπτομέρειες του μηνύματος, το οποίο περιλαμβάνει το Αναγνωριστικό μηνύματος.</span><span class="sxs-lookup"><span data-stu-id="df8f6-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="df8f6-108">Σημειώστε ότι η σύνδεση της εξερεύνησης απειλών θα φιλτράρει αυτόματα τα μηνύματα που αντιστοιχούν στα κριτήρια ειδοποίησης.</span><span class="sxs-lookup"><span data-stu-id="df8f6-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="df8f6-109">Ίσως χρειαστεί να προσαρμόσετε το φίλτρο ημερομηνίας στην Εξερεύνηση απειλών.</span><span class="sxs-lookup"><span data-stu-id="df8f6-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="df8f6-110">Το μήνυμα ηλεκτρονικού "ψαρέματος" παραδόθηκε λόγω παράκαμψης που έχει ρυθμιστεί με μη αυτόματο τρόπο:</span><span class="sxs-lookup"><span data-stu-id="df8f6-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="df8f6-111">Ένας επιτρεπόμενος αποστολέας ή τομέας που έχει καθοριστεί από το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="df8f6-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="df8f6-112">Ένας επιτρεπόμενος αποστολέας ή τομέας που έχει καθοριστεί από τον διαχειριστή σε μια πολιτική αντι-ανεπιθύμητης αλληλογραφίας.</span><span class="sxs-lookup"><span data-stu-id="df8f6-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="df8f6-113">Μια επιτρεπόμενη διεύθυνση IP σε μια πολιτική φίλτρου σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="df8f6-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="df8f6-114">Ένας κανόνας ροής αλληλογραφίας (γνωστό και ως κανόνας μεταφοράς) που έχει ρυθμιστεί ώστε να επιτρέπει την είσοδο σε μηνύματα.</span><span class="sxs-lookup"><span data-stu-id="df8f6-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="df8f6-115">Εάν πιστεύετε ότι το μήνυμα έχει επισημανθεί εσφαλμένα ως "Phish", χρησιμοποιήστε το [πρόσθετο μήνυμα αναφοράς](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) του Outlook για να υποβάλετε δείγματα μηνυμάτων στη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="df8f6-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
