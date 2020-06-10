---
title: Kaizala Pro サブスクリプションを Microsoft365 に移行する
description: Kaizala Pro サブスクリプションを Microsoft365 または Office 365 バージョンに移行する方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611238"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="887c2-103">Kaizala Pro スタンドアロンサブスクリプションを Microsoft365 または Office 365 バージョンに移行する</span><span class="sxs-lookup"><span data-stu-id="887c2-103">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="887c2-104">2020年7月1日より、Microsoft は Kaizala Pro スタンドアロンサービスの売上を終了します。</span><span class="sxs-lookup"><span data-stu-id="887c2-104">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="887c2-105">お客様は、この日より後に新しい Kaizala Pro サブスクリプションを購入することはできなくなります。また、既存の Kaizala Pro サブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="887c2-105">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="887c2-106">お客様の継続性を確保するには、Kaizala Pro スタンドアロンサブスクリプションが期限切れになっているお客様を、サポートされている SKU オプション (下記参照) に移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="887c2-106">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="887c2-107">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="887c2-107">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="887c2-108">API (CREST またはパートナーセンター) を使用する場合、[自動更新] プロパティを false に設定して、サブスクリプションの終了日を評価することで、期限切れのサブスクリプションを検出できます `auto renew = False` 。</span><span class="sxs-lookup"><span data-stu-id="887c2-108">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="887c2-109">E4 サブスクリプションは `auto renew=False` 、2020年7月1日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="887c2-109">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="887c2-110">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="887c2-110">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="887c2-111">Kaizala Pro スタンドアロン置換プラン</span><span class="sxs-lookup"><span data-stu-id="887c2-111">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="887c2-112">新しいプランでは、お客様は Microsoft 365 の新しい機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="887c2-112">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="887c2-113">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="887c2-113">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="887c2-114">次を含む[**ビジネス向け Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2):</span><span class="sxs-lookup"><span data-stu-id="887c2-114">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="887c2-115">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="887c2-115">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="887c2-116">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="887c2-116">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="887c2-117">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="887c2-117">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="887c2-118">[**最前線の Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)(次を含む):</span><span class="sxs-lookup"><span data-stu-id="887c2-118">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="887c2-119">Microsoft 365 F3 (旧称 Microsoft 365 F1) と Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="887c2-119">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="887c2-120">以下を含む、 [**Enterprise の Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans):</span><span class="sxs-lookup"><span data-stu-id="887c2-120">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="887c2-121">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="887c2-121">Office 365 E1</span></span>
   - <span data-ttu-id="887c2-122">Microsoft 365 E3 と Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="887c2-122">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="887c2-123">Microsoft 365 E5 と Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="887c2-123">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="887c2-124">以下を含む[**教育の Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365):</span><span class="sxs-lookup"><span data-stu-id="887c2-124">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="887c2-125">Microsoft 365 A1 と Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="887c2-125">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="887c2-126">Microsoft 365 A3 と Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="887c2-126">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="887c2-127">Microsoft 365 A5 と Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="887c2-127">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="887c2-128">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="887c2-128">Transition customers to new product plans</span></span>

<span data-ttu-id="887c2-129">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="887c2-129">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="887c2-130">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="887c2-130">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="887c2-131">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="887c2-131">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="887c2-132">A.</span><span class="sxs-lookup"><span data-stu-id="887c2-132">A.</span></span> <span data-ttu-id="887c2-133">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="887c2-133">Purchase the new subscription</span></span>

<span data-ttu-id="887c2-134">B.</span><span class="sxs-lookup"><span data-stu-id="887c2-134">B.</span></span> <span data-ttu-id="887c2-135">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="887c2-135">Reassign current user licenses</span></span>

<span data-ttu-id="887c2-136">C.</span><span class="sxs-lookup"><span data-stu-id="887c2-136">C.</span></span> <span data-ttu-id="887c2-137">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="887c2-137">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="887c2-138">新しいプランにお客様を移行する</span><span class="sxs-lookup"><span data-stu-id="887c2-138">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="887c2-139">A.</span><span class="sxs-lookup"><span data-stu-id="887c2-139">A.</span></span> <span data-ttu-id="887c2-140">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="887c2-140">Purchase the new subscription</span></span>

1. <span data-ttu-id="887c2-141">新しいサブスクリプションを購入するには、**パートナーセンター**メニューから [**顧客**] を選択し、移動する顧客を選択して、[**サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-141">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="887c2-142">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="887c2-142">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="887c2-143">お客様は、以前のサブスクリプションと新しいサブスクリプション (オプション 1-Office 365 Enterprise F1 など) の両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="887c2-143">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="887c2-144">B.</span><span class="sxs-lookup"><span data-stu-id="887c2-144">B.</span></span> <span data-ttu-id="887c2-145">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="887c2-145">Reassign current user licenses</span></span>

1. <span data-ttu-id="887c2-146">顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="887c2-146">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="887c2-147">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="887c2-147">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="887c2-148">ユーザーライセンスを再割り当てするには、再割り当てするユーザーを選択し、[**ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-148">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="887c2-149">[**ライセンスの管理**] ページで、[Kaizala Pro スタンドアロンライセンス] チェックボックスをオフにし、顧客の移動先のサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-149">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="887c2-150">**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-150">Select **Submit**.</span></span> <span data-ttu-id="887c2-151">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="887c2-151">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="887c2-152">ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。</span><span class="sxs-lookup"><span data-stu-id="887c2-152">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="887c2-153">C.</span><span class="sxs-lookup"><span data-stu-id="887c2-153">C.</span></span> <span data-ttu-id="887c2-154">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="887c2-154">Cancel old subscription</span></span>

<span data-ttu-id="887c2-155">ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="887c2-155">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="887c2-156">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-156">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="887c2-157">サブスクリプションをキャンセルする顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-157">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="887c2-158">サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="887c2-158">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="887c2-159">**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="887c2-159">Select **Submit**.</span></span>

<span data-ttu-id="887c2-160">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="887c2-160">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="887c2-161">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="887c2-161">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="887c2-162">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="887c2-162">The customer incurs no additional costs for the old subscription.</span></span>