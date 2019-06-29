---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388245"
---
<span data-ttu-id="30956-103">Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.</span><span class="sxs-lookup"><span data-stu-id="30956-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="30956-104">**Κλειδί μητρώου**</span><span class="sxs-lookup"><span data-stu-id="30956-104">**Registry key**</span></span>|<span data-ttu-id="30956-105">**Τύπος**</span><span class="sxs-lookup"><span data-stu-id="30956-105">**Type**</span></span>|<span data-ttu-id="30956-106">**Τιμή**</span><span class="sxs-lookup"><span data-stu-id="30956-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="30956-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="30956-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="30956-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="30956-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="30956-109">1</span><span class="sxs-lookup"><span data-stu-id="30956-109">1</span></span>  <br/> |

<span data-ttu-id="30956-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="30956-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="30956-111">ADAL είναι ενεργοποιημένη από προεπιλογή στο Office 365 ProPlus και Office 2016.</span><span class="sxs-lookup"><span data-stu-id="30956-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="30956-112">> Υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ήταν προηγουμένως με το όνομα των υπηρεσιών Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="30956-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  