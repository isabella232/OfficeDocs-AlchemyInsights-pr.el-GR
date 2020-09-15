---
title: η υπηρεσία του 1048 5.7.750 δεν είναι διαθέσιμη. Το πρόγραμμα-πελάτης αποκλειστεί από την αποστολή από μη καταχωρημένους τομείς
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664242"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="afa2c-103">το πρόγραμμα-πελάτης 5.7.750 αποκλειστεί από την αποστολή από μη καταχωρημένο τομέα</span><span class="sxs-lookup"><span data-stu-id="afa2c-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="afa2c-104">Το σφάλμα παρουσιάζεται όταν ένας μεγάλος όγκος μηνυμάτων αποστέλλονται από τομείς που δεν έχουν παρασχεθεί στον μισθωτή σας (προστίθενται ως αποδεκτοί τομείς και επικυρωμένοι).</span><span class="sxs-lookup"><span data-stu-id="afa2c-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="afa2c-105">Για να αποφύγετε αυτό το σφάλμα, μπορείτε να χρησιμοποιήσετε μια σύνδεση ροής αλληλογραφίας που βασίζεται σε πιστοποιητικά, όπου ο τομέας του πιστοποιητικού είναι ένας τομέας που έχει παρασχεθεί ή μπορείτε να προβλεφθούν όλοι οι τομείς αποστολής.</span><span class="sxs-lookup"><span data-stu-id="afa2c-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
