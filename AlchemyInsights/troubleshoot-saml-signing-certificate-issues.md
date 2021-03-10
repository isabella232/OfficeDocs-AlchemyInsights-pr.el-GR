---
title: Αντιμετώπιση προβλημάτων πιστοποιητικού υπογραφής SAML
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
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693421"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="e3509-102">Αντιμετώπιση προβλημάτων πιστοποιητικού υπογραφής SAML</span><span class="sxs-lookup"><span data-stu-id="e3509-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="e3509-103">Για να επιλύσετε το ζήτημα του πιστοποιητικού υπογραφής SAML, εκτελέστε τα ακόλουθα προτεινόμενα βήματα:</span><span class="sxs-lookup"><span data-stu-id="e3509-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="e3509-104">Όταν προσθέτετε μια εταιρική εφαρμογή που υποστηρίζει SSO, το Azure θα δημιουργήσει ένα πιστοποιητικό που ονομάζεται [πιστοποιητικό υπογραφής SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="e3509-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="e3509-105">Αυτό το πιστοποιητικό έχει ημερομηνία λήξης 3 ετών.</span><span class="sxs-lookup"><span data-stu-id="e3509-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="e3509-106">Για να αλλάξετε την ημερομηνία λήξης του πιστοποιητικού, ανατρέξτε στο θέμα "Προσαρμογή της ημερομηνίας λήξης για το πιστοποιητικό ομοσπονδίας και [αναδίφτε το σε νέο πιστοποιητικό".](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="e3509-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="e3509-107">Το Azure θα χρησιμοποιήσει αυτό το πιστοποιητικό για να υπογράψει τα διακριτικά SAML που ζητούνται από την εφαρμογή και να τα στείλει στην εφαρμογή για μια επιτυχημένη SSO.</span><span class="sxs-lookup"><span data-stu-id="e3509-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="e3509-108">Για να ολοκληρωθεί αυτό, κάντε λήψη του πιστοποιητικού από την πύλη Azure και στείλτε το στον προμηθευτή της εφαρμογής για να ολοκληρώσετε τη διαδικασία SSO.</span><span class="sxs-lookup"><span data-stu-id="e3509-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="e3509-109">Αφού ολοκληρωθεί αυτή η διαδικασία, η εφαρμογή σας θα εμπιστευτεί αυτό το πιστοποιητικό και όλα τα διακριτικά SAML που είναι υπογεγραμμένα από αυτό το πιστοποιητικό θα γίνουν αποδεκτά από την εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="e3509-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="e3509-110">Εάν λήξει αυτό το πιστοποιητικό, δημιουργήστε ένα νέο πιστοποιητικό, ενημερώστε το στον προμηθευτή της εφαρμογής και, στη συνέχεια, ενεργές στην πλευρά Azure.</span><span class="sxs-lookup"><span data-stu-id="e3509-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="e3509-111">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Ανανέωση πιστοποιητικού που σύντομα θα λήξει".](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="e3509-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="e3509-112">Εάν λήξει το πιστοποιητικό, ο χρήστης δεν θα αποκλειστεί.</span><span class="sxs-lookup"><span data-stu-id="e3509-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="e3509-113">[Προσθέστε μια διεύθυνση ηλεκτρονικού ταχυδρομείου για να λαμβάνετε](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) ειδοποιήσεις πριν από τη λήξη του τρέχοντος πιστοποιητικού.</span><span class="sxs-lookup"><span data-stu-id="e3509-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="e3509-114">Το βήμα 4 είναι προαιρετικό.</span><span class="sxs-lookup"><span data-stu-id="e3509-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="e3509-115">Αλλάξτε τις επιλογές υπογραφής πιστοποιητικών SAML μιας εφαρμογής και τον αλγόριθμο υπογραφής πιστοποιητικού.</span><span class="sxs-lookup"><span data-stu-id="e3509-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="e3509-116">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα ["Αλλαγή επιλογών υπογραφής πιστοποιητικού και αλγόριθμος υπογραφής".](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="e3509-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

