---
title: Αντιμετώπιση προβλημάτων απρόσκοπτης μεμονωμένης σύνδεσης (SSO) για εσωτερική εγκατάσταση
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816210"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="317f4-102">Αντιμετώπιση προβλημάτων απρόσκοπτης μεμονωμένης σύνδεσης (SSO) για εσωτερική εγκατάσταση</span><span class="sxs-lookup"><span data-stu-id="317f4-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="317f4-103">Για να επιλύσετε προβλήματα απλής σύνδεσης (SSO), ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="317f4-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="317f4-104">**Πώς μπορώ να κάνω επαναφορά του κλειδιού αποκρυπτογράφησης Kerberos του λογαριασμού υπολογιστή AZUREADSSO;**</span><span class="sxs-lookup"><span data-stu-id="317f4-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="317f4-105">Συνιστάται ιδιαίτερα να κάνετε επαναφορά του κλειδιού αποκρυπτογράφησης Kerberos τουλάχιστον κάθε 30 ημέρες.</span><span class="sxs-lookup"><span data-stu-id="317f4-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="317f4-106">Για να το κάνετε αυτό με μη αυτόματο τρόπο, ανατρέξτε στο θέμα Τρόπος [επαναφοράς των πλήκτρων αποκρυπτογράφησης Kerberos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)</span><span class="sxs-lookup"><span data-stu-id="317f4-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="317f4-107">**Ρύθμιση παραμέτρων απρόσκοπτη SSO**</span><span class="sxs-lookup"><span data-stu-id="317f4-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="317f4-108">Για να αναπτύξετε απρόσκοπτη SSO, ακολουθήστε τα βήματα στο [Azure Active Directory Απρόσκοπτη ενιαία σύνδεση: Γρήγορη εκκίνηση.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)</span><span class="sxs-lookup"><span data-stu-id="317f4-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="317f4-109">**Συμβουλευτικές υπηρεσίες**</span><span class="sxs-lookup"><span data-stu-id="317f4-109">**Advisory**</span></span>

- <span data-ttu-id="317f4-110">[Απλή σύνδεση του Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) Συνήθεις ερωτήσεις - Σε αυτό το άρθρο, θα αντιμετωπίσουμε συνήθεις ερωτήσεις σχετικά με το Azure Active Directory Seamless Single Sign-On (Απρόσκοπτη SSO).</span><span class="sxs-lookup"><span data-stu-id="317f4-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="317f4-111">Συνεχίστε να ελέγχετε για νέο περιεχόμενο.</span><span class="sxs-lookup"><span data-stu-id="317f4-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="317f4-112">[Ερωτήσεις&Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τον τρόπο υποβολής αιτήσεων δυνατοτήτων ή υποβολής τεχνικών ερωτήσεων σχετικά με την απρόσκοπτη SSO.</span><span class="sxs-lookup"><span data-stu-id="317f4-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="317f4-113">**Αντιμετώπιση προβλημάτων**</span><span class="sxs-lookup"><span data-stu-id="317f4-113">**Troubleshoot**</span></span>

<span data-ttu-id="317f4-114">[Αντιμετώπιση προβλημάτων](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) της απλής σύνδεσης του Azure Active Directory - Αυτό το άρθρο σάς βοηθά να βρείτε πληροφορίες αντιμετώπισης προβλημάτων σχετικά με συνήθη προβλήματα σχετικά με το Azure Active Directory (Azure AD) Απρόσκοπτη ενιαία Sign-On (Απρόσκοπτη SSO).</span><span class="sxs-lookup"><span data-stu-id="317f4-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







