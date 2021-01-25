---
title: Υποβολή ερωτημάτων στο Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974417"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="396e0-102">Υποβολή ερωτημάτων στο Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="396e0-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="396e0-103">Αυτό το θέμα μπορεί επίσης να ισχύει για προγραμματιστές που εξακολουθούν να χρησιμοποιούν το API AD Graph του Azure.</span><span class="sxs-lookup"><span data-stu-id="396e0-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="396e0-104">Ωστόσο, συνιστάται **ανεπιφύλακτα** να χρησιμοποιείτε το Microsoft Graph για όλα τα σενάρια καταλόγου, ταυτότητας και διαχείρισης πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="396e0-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="396e0-105">**Ζητήματα ελέγχου ταυτότητας ή εξουσιοδότησης**</span><span class="sxs-lookup"><span data-stu-id="396e0-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="396e0-106">Εάν η εφαρμογή σας **δεν μπορεί να αποκτήσει διακριτικά** για να καλεί το Microsoft Graph, επιλέξτε **πρόβλημα με τη λήψη μιας κατηγορίας διακριτικού πρόσβασης (έλεγχος ταυτότητας)** του Microsoft Graph για να λάβετε πιο συγκεκριμένη βοήθεια και υποστήριξη για αυτό το θέμα.</span><span class="sxs-lookup"><span data-stu-id="396e0-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="396e0-107">Εάν η εφαρμογή σας **λαμβάνει σφάλματα εξουσιοδότησης του 401 ή του 403** κατά την κλήση του Microsoft Graph, επιλέξτε την κατηγορία API του Microsoft Graph με **δυνατότητα πρόσβασης (εξουσιοδότηση)** για να λάβετε πιο συγκεκριμένη βοήθεια και υποστήριξη για αυτό το θέμα.</span><span class="sxs-lookup"><span data-stu-id="396e0-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="396e0-108">**Θέλω να χρησιμοποιήσω το Microsoft Graph, αλλά δεν είμαι σίγουρος από πού να ξεκινήσω**</span><span class="sxs-lookup"><span data-stu-id="396e0-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="396e0-109">Για να μάθετε περισσότερα σχετικά με το Microsoft Graph, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="396e0-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="396e0-110">Επισκόπηση του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="396e0-111">Επισκόπηση της διαχείρισης ταυτοτήτων και πρόσβασης στο Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="396e0-112">Γρήγορα αποτελέσματα με τη δημιουργία εφαρμογών του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="396e0-113">**Εξερεύνηση του Microsoft Graph** -Ελέγξτε τα API του Microsoft Graph στον μισθωτή σας ή σε έναν μισθωτή demo</span><span class="sxs-lookup"><span data-stu-id="396e0-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="396e0-114">**Θέλω να χρησιμοποιήσω το Microsoft Graph, αλλά υποστηρίζει τα API καταλόγου v 1.0 που χρειάζομαι;**</span><span class="sxs-lookup"><span data-stu-id="396e0-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="396e0-115">Το Microsoft Graph είναι το προτεινόμενο API για τον κατάλογο, την ταυτότητα και τη διαχείριση πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="396e0-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="396e0-116">Ωστόσο, εξακολουθούν να υπάρχουν μερικά κενά μεταξύ του τι είναι δυνατό στο Azure AD Graph και το Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="396e0-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="396e0-117">Εξετάστε τα ακόλουθα άρθρα, τα οποία τονίζουν τις πιο πρόσφατες διαφορές που πρέπει να βοηθήσετε στην επιλογή σας:</span><span class="sxs-lookup"><span data-stu-id="396e0-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="396e0-118">Διαφορές τύπου πόρου μεταξύ του Azure AD Graph και του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="396e0-119">Διαφορές ιδιοτήτων μεταξύ του Azure AD Graph και του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="396e0-120">Διαφορές μεθόδου μεταξύ του Azure AD και του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="396e0-121">**Όταν κάνω ερώτημα στο αντικείμενο *χρήστη* , πολλές από τις ιδιότητές του λείπουν**</span><span class="sxs-lookup"><span data-stu-id="396e0-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="396e0-122">`GET https://graph.microsoft.com/v1.0/users` επιστρέφει μόνο 11 ιδιότητες, καθώς το Microsoft Graph κάνει αυτόματη επιλογή ενός προεπιλεγμένου συνόλου ιδιοτήτων *χρήστη* για να επιστρέψει.</span><span class="sxs-lookup"><span data-stu-id="396e0-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="396e0-123">Εάν χρειάζεστε άλλες ιδιότητες *χρήστη* , χρησιμοποιήστε το $Select για να επιλέξετε τις ιδιότητες που χρειάζεται η εφαρμογή σας.</span><span class="sxs-lookup"><span data-stu-id="396e0-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="396e0-124">Δοκιμάστε το πρώτα στο **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="396e0-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="396e0-125">**Ορισμένες τιμές ιδιοτήτων χρήστη είναι *Null* , παρόλο που γνωρίζω ότι έχουν καθοριστεί**</span><span class="sxs-lookup"><span data-stu-id="396e0-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="396e0-126">Η πιο πιθανή εξήγηση είναι ότι η εφαρμογή είχε εκχωρηθεί στο *χρήστη. ReadBasic. All* permission.</span><span class="sxs-lookup"><span data-stu-id="396e0-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="396e0-127">Με αυτόν τον τρόπο, η εφαρμογή μπορεί να διαβάσει ένα περιορισμένο σύνολο ιδιοτήτων χρήστη, επιστρέφοντας όλες τις άλλες ιδιότητες ως null, ακόμα και αν έχουν οριστεί προηγουμένως.</span><span class="sxs-lookup"><span data-stu-id="396e0-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="396e0-128">Δοκιμάστε να εκχωρήσετε στο χρήστη την εφαρμογή *. Read. All* permission αντ ' αυτού.</span><span class="sxs-lookup"><span data-stu-id="396e0-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="396e0-129">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [δικαιώματα χρήστη του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="396e0-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="396e0-130">**Αντιμετωπίζω προβλήματα με τη χρήση παραμέτρων ερωτημάτων OData για το φιλτράρισμα δεδομένων στις αιτήσεις μου**</span><span class="sxs-lookup"><span data-stu-id="396e0-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="396e0-131">Ενώ το Microsoft Graph υποστηρίζει ένα ευρύ φάσμα των παραμέτρων του ερωτήματος OData, πολλές από αυτές τις παραμέτρους δεν υποστηρίζονται πλήρως από τις υπηρεσίες καταλόγου (πόροι που κληρονομούν από το *directoryObject*) στο Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="396e0-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="396e0-132">Οι ίδιοι περιορισμοί που υπήρχαν στο Azure AD Graph επιμένουν για το μεγαλύτερο μέρος του Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="396e0-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="396e0-133">**Δεν υποστηρίζεται**: $count, $search και $Filter σε τιμές *Null* ή *Not Null*</span><span class="sxs-lookup"><span data-stu-id="396e0-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="396e0-134">**Δεν υποστηρίζεται**: $Filter σε ορισμένες ιδιότητες (ανατρέξτε στο θέμα θέματα πόρων στα οποία οι ιδιότητες είναι φιλτραρισμένες)</span><span class="sxs-lookup"><span data-stu-id="396e0-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="396e0-135">**Δεν υποστηρίζεται**: σελιδοποίηση, φιλτράρισμα και ταξινόμηση την ίδια στιγμή</span><span class="sxs-lookup"><span data-stu-id="396e0-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="396e0-136">**Δεν υποστηρίζεται**: φιλτράρισμα σε σχέση.</span><span class="sxs-lookup"><span data-stu-id="396e0-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="396e0-137">Για παράδειγμα-Εντοπίστε όλα τα μέλη της ομάδας μηχανικών που βρίσκονται στο Ηνωμένο Βασίλειο.</span><span class="sxs-lookup"><span data-stu-id="396e0-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="396e0-138">**Μερική υποστήριξη**: $OrderBy στο *χρήστη* (μόνο για εμφανιζόμενο όνομα και UserPrincipalName) και στην *ομάδα*</span><span class="sxs-lookup"><span data-stu-id="396e0-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="396e0-139">**Μερική υποστήριξη**: $Filter (υποστηρίζει μόνο την υποστήριξη *EQ*,  *startswith* ή *και και* περιορισμένη *οποιαδήποτε*), $Expand (η επέκταση των σχέσεων ενός αντικειμένου επιστρέφει όλες τις σχέσεις, αλλά η επέκταση μιας συλλογής των σχέσεων αντικειμένων είναι περιορισμένη)</span><span class="sxs-lookup"><span data-stu-id="396e0-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="396e0-140">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Προσαρμογή απαντήσεων με παραμέτρους ερωτήματος](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="396e0-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="396e0-141">**Το API που καλώ δεν λειτουργεί-πού μπορώ να κάνω περισσότερες δοκιμές;**</span><span class="sxs-lookup"><span data-stu-id="396e0-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="396e0-142">**Εξερεύνηση του Microsoft Graph** -δοκιμάστε τα API του Microsoft Graph στον μισθωτή σας ή σε έναν μισθωτή demo και δείτε επίσης τα **δείγματα ερωτημάτων** στην Εξερεύνηση του Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="396e0-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="396e0-143">**Όταν κάνω ερώτημα για δεδομένα, φαίνεται σαν να έχω μια ελλιπή επαναφορά δεδομένων**</span><span class="sxs-lookup"><span data-stu-id="396e0-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="396e0-144">Εάν κάνετε αναζήτηση σε μια συλλογή (όπως *οι χρήστες*), το Microsoft Graph χρησιμοποιεί όρια σελίδας από την πλευρά του διακομιστή, ώστε τα αποτελέσματα να επιστρέφονται πάντα με ένα προεπιλεγμένο μέγεθος σελίδας.</span><span class="sxs-lookup"><span data-stu-id="396e0-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="396e0-145">Η εφαρμογή σας θα πρέπει πάντα να αναμένει τη σελίδα μέσω συλλογών που επιστρέφονται από την υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="396e0-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="396e0-146">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="396e0-146">For more information, see:</span></span>

- [<span data-ttu-id="396e0-147">Βέλτιστες πρακτικές του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="396e0-148">Σελιδοποίηση δεδομένων του Microsoft Graph στην εφαρμογή σας</span><span class="sxs-lookup"><span data-stu-id="396e0-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="396e0-149">**Η εφαρμογή μου είναι πολύ αργή και γίνεται επίσης επιτάχυνση. Ποιες βελτιώσεις μπορώ να κάνω;**</span><span class="sxs-lookup"><span data-stu-id="396e0-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="396e0-150">Ανάλογα με το σενάριό σας, υπάρχουν διάφορες επιλογές που έχετε στη διάθεσή σας για να κάνετε την εφαρμογή σας πιο εκτελεστή και, σε ορισμένες περιπτώσεις, λιγότερο επιρρεπής στο να ρυθμίζεται από την υπηρεσία (όταν πραγματοποιείτε πάρα πολλές κλήσεις).</span><span class="sxs-lookup"><span data-stu-id="396e0-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="396e0-151">Για να μάθετε περισσότερα, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="396e0-151">To learn more, see:</span></span>

- [<span data-ttu-id="396e0-152">Βέλτιστες πρακτικές του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="396e0-153">Μαζικές αιτήσεις</span><span class="sxs-lookup"><span data-stu-id="396e0-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="396e0-154">Παρακολούθηση αλλαγών μέσω ερωτήματος Δέλτα</span><span class="sxs-lookup"><span data-stu-id="396e0-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="396e0-155">Ενημερωθείτε για τις αλλαγές μέσω των άγκιστρων</span><span class="sxs-lookup"><span data-stu-id="396e0-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="396e0-156">Καθοδήγηση περιορισμού</span><span class="sxs-lookup"><span data-stu-id="396e0-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="396e0-157">**Πού μπορώ να βρω περισσότερες πληροφορίες σχετικά με σφάλματα και γνωστά προβλήματα;**</span><span class="sxs-lookup"><span data-stu-id="396e0-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="396e0-158">Πληροφορίες απόκρισης σφάλματος του Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="396e0-159">Γνωστά θέματα με το Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="396e0-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="396e0-160">**Πού μπορώ να ελέγχω την κατάσταση διαθεσιμότητας και συνδεσιμότητας υπηρεσίας;**</span><span class="sxs-lookup"><span data-stu-id="396e0-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="396e0-161">Η διαθεσιμότητα και η συνδεσιμότητα υπηρεσιών των υποκείμενων υπηρεσιών στις οποίες είναι δυνατή η πρόσβαση μέσω του Microsoft Graph μπορεί να επηρεάσει τη συνολική διαθεσιμότητα και τις επιδόσεις του Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="396e0-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="396e0-162">Για την εύρυθμη λειτουργία της υπηρεσίας καταλόγου Active Directory Azure, ανατρέξτε στην κατάσταση των υπηρεσιών **ταυτότητας Security +** που παρατίθενται στη [σελίδα κατάστασης Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="396e0-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="396e0-163">Για τις υπηρεσίες του Office που συμβάλλουν στο Microsoft Graph, ανατρέξτε στην κατάσταση των υπηρεσιών που παρατίθενται στον [πίνακα εργαλείων εύρυθμης λειτουργίας της υπηρεσίας Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="396e0-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
