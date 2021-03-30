---
title: Λήψη λίστας εταιρικών εφαρμογών
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404932"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="556c9-102">Λήψη λίστας εταιρικών εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="556c9-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="556c9-103">Για να λάβετε **μια** λίστα των εταιρικών εφαρμογών (όλες οι εφαρμογές ή φιλτραρισμένο κατά εμφανιζόμενο όνομα, αναγνωριστικό, διευθύνσεις URL αναγνωριστικού κ.λπ.) μέσω της εντολής Powershell, ανατρέξτε στο θέμα [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="556c9-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="556c9-104">Για να λάβετε μια λίστα με τα κύρια αντικείμενα υπηρεσίας (όλα τα αντικείμενα ή φιλτραρισμένο κατά αναγνωριστικό) μέσω της εντολής Powershell, ανατρέξτε στο θέμα [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="556c9-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="556c9-105">Εάν θέλετε να λάβετε μια **λίστα με τις ρυθμισμένες εφαρμογές SAML, οι ακόλουθες δέσμες ενεργειών του PowerShell μπορεί** να σας βοηθήσουν:</span><span class="sxs-lookup"><span data-stu-id="556c9-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="556c9-106">Κάθε εφαρμογή είτε είναι μια εφαρμογή OAuth είτε μια εφαρμογή SAML (εφαρμογές συλλογής και εφαρμογές που δεν είναι συλλογή) θα έχουν δύο αντικείμενα που δημιουργούνται στο AAD όταν συμβεί η εγγραφή τους.</span><span class="sxs-lookup"><span data-stu-id="556c9-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="556c9-107">Το ένα ονομάζεται αντικείμενο εφαρμογής και το άλλο είναι το αντικείμενο Service Principal.</span><span class="sxs-lookup"><span data-stu-id="556c9-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="556c9-108">Όταν τοποθετείτε σε απόρριψη τις ιδιότητες ενός κύριου αντικειμένου υπηρεσίας χρησιμοποιώντας το PowerShell, θα βρείτε ότι κάθε εφαρμογή έχει έναν συγκεκριμένο αριθμό ετικετών που σχετίζονται με αυτό, όπως:</span><span class="sxs-lookup"><span data-stu-id="556c9-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="556c9-109">Οι εφαρμογές OAuth θα έχουν μια ετικέτα που ονομάζεται "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="556c9-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="556c9-110">Οι εφαρμογές SAML συλλογής θα έχουν μια ετικέτα που ονομάζεται "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="556c9-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="556c9-111">Οι εφαρμογές SAML που δεν είναι συλλογής θα έχουν μια ετικέτα που ονομάζεται "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="556c9-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="556c9-112">Ως εκ τούτου, μπορείτε να χρησιμοποιήσετε αυτές τις ετικέτες και να μάθετε τι είδους εφαρμογή είναι.</span><span class="sxs-lookup"><span data-stu-id="556c9-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="556c9-113">Η ετικέτα **"WindowsAzureActiveDirectoryIntegratedApp"** είναι συνηθισμένη σε όλους τους τύπους εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="556c9-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="556c9-114">Μπορείτε να χρησιμοποιήσετε το ακόλουθο τμήμα για να παρατίθενται όλες οι εφαρμογές SAML (συλλογή και μη συλλογή):</span><span class="sxs-lookup"><span data-stu-id="556c9-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="556c9-115">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Αναγνώριση εφαρμογών με δυνατότητα SAML στο Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="556c9-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="556c9-116">**Εύρεση και λίστα μόνο εφαρμογών Web:** Χρησιμοποιήστε την παρακάτω εντολή για να λάβετε όλες τις εφαρμογές Azure AD με τον τύπο εφαρμογής "Εφαρμογή Web/API"</span><span class="sxs-lookup"><span data-stu-id="556c9-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="556c9-117">Get-AzureADApplication -Όλα:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="556c9-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="556c9-118">**Εύρεση και λίστα εγγενών εφαρμογών** μόνο: Εκτελέστε την ακόλουθη εντολή για να λάβετε όλες τις εγγενείς εφαρμογές προγράμματος-πελάτη (υπολογιστή/κινητής συσκευής).</span><span class="sxs-lookup"><span data-stu-id="556c9-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="556c9-119">Get-AzureADApplication -Όλα:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="556c9-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="556c9-120">**Εξαγωγή όλων των καταχωρημένων λεπτομερειών εφαρμογής Azure AD στο CSV:** Η παρακάτω εντολή εξάγει όλες τις εφαρμογές Azure AD με απαιτούμενες λεπτομέρειες στο αρχείο csv:</span><span class="sxs-lookup"><span data-stu-id="556c9-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="556c9-121">Get-AzureADApplication -Όλα:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="556c9-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="556c9-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Κωδικοποίηση UTF8</span><span class="sxs-lookup"><span data-stu-id="556c9-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="556c9-123">**Πρέπει να εξαγάγετε μια λίστα των εφαρμογών Azure που δεν τίθενται σε χρήση** – Αναφορά ελέγχου</span><span class="sxs-lookup"><span data-stu-id="556c9-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="556c9-124">Το Azure AD μπορεί να εμφανίζει αρχεία καταγραφής εφαρμογών μόνο για έως και 30 ημέρες, με την προϋπόθεση ότι έχετε άδεια χρήσης Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="556c9-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="556c9-125">Έχετε δύο επιλογές για να διατηρήσετε τα δεδομένα για περισσότερο από 30 ημέρες.</span><span class="sxs-lookup"><span data-stu-id="556c9-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="556c9-126">Μπορείτε να χρησιμοποιήσετε τα [API αναφοράς AZURE AD για](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) να ανακτήσετε τα δεδομένα μέσω προγραμματισμού και να τα αποθηκεύσετε σε μια βάση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="556c9-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="556c9-127">Εναλλακτικά, μπορείτε να ενσωματώσετε αρχεία καταγραφής ελέγχου σε ένα σύστημα SIEM άλλου κατασκευαστή.</span><span class="sxs-lookup"><span data-stu-id="556c9-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="556c9-128">Μπορείτε επίσης να κάνετε λήψη της λίστας εφαρμογών για όλες τις εφαρμογές και τις εφαρμογές που ανήκουν στο Azure Active Directory>Καταχωρήσεις εφαρμογών>Λήψη>Όλες οι εφαρμογές/οι εφαρμογές που ανήκουν.</span><span class="sxs-lookup"><span data-stu-id="556c9-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="556c9-129">Για να λάβετε μια λίστα εφαρμογών μέσω του MS Graph, ανατρέξτε στο θέμα Εφαρμογές λίστας [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) και τύπος πόρου [εφαρμογής - Microsoft Graph v1.0.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="556c9-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
