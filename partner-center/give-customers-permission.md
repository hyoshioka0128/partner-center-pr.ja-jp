---
title: 顧客が個人でサービスを購入するためのアクセス許可を付与する
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムパートナーが、お客様が購入したサブスクリプションに対して Azure の予約などの独自のサービスを購入できるようにする方法について説明します。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: サブスクリプション、セルフサービス型購入、セルフサービス RI、有効化 ri、無効化 RI、セルフサービス、顧客購入、カスタマーアクセス許可、顧客購入予約インスタンス、顧客購入 Azure 予約、セルフサービスの有効化、セルフサービスの無効化
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255464"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a><span data-ttu-id="53a05-104">顧客が自分の製品またはサービスを購入するためのアクセス許可を付与する方法について説明します</span><span class="sxs-lookup"><span data-stu-id="53a05-104">Learn how to give customers permission to buy their own products or services</span></span>

<span data-ttu-id="53a05-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="53a05-105">**Applies to**</span></span>

- <span data-ttu-id="53a05-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="53a05-106">Partner Center</span></span>
- <span data-ttu-id="53a05-107">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="53a05-107">Partners in the CSP program</span></span>

<span data-ttu-id="53a05-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="53a05-108">**Appropriate roles**</span></span>

- <span data-ttu-id="53a05-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="53a05-109">Admin agent</span></span>
- <span data-ttu-id="53a05-110">販売代理店</span><span class="sxs-lookup"><span data-stu-id="53a05-110">Sales agent</span></span>

<span data-ttu-id="53a05-111">この記事では、クラウドソリューションプロバイダー (CSP) プログラムのパートナーが、独自のサービスまたはリソースの一部を購入するためのアクセス許可を付与する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="53a05-111">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="53a05-112">CSP プログラムのパートナーは、多くの場合、パートナーセンターとその商用マーケットプレースを使用して、顧客向けのソリューションとサービスを購入します。</span><span class="sxs-lookup"><span data-stu-id="53a05-112">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="53a05-113">パートナーは、一部のお客様に対して、これらのサービスを Azure portal から直接プロビジョニングすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="53a05-113">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="53a05-114">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="53a05-114">Here's an example.</span></span> <span data-ttu-id="53a05-115">たとえば、パートナーセンターで顧客の Azure プランサブスクリプションを購入したとします。</span><span class="sxs-lookup"><span data-stu-id="53a05-115">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="53a05-116">その後、顧客の代理として、そのサブスクリプションに他のリソースまたはサービスを追加することを決定します。</span><span class="sxs-lookup"><span data-stu-id="53a05-116">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="53a05-117">この場合、顧客のサブスクリプションに Azure の予約を追加することができます (予約済みの仮想マシンインスタンスの追加など)。</span><span class="sxs-lookup"><span data-stu-id="53a05-117">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="53a05-118">その後、顧客が Azure portal で Azure 予約リソースをさらにプロビジョニングできるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-118">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="53a05-119">これで、**顧客のアクセス許可**機能を使用して、Azure リソースでより多くのセルフサービスオプションをお客様に提供できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="53a05-119">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="53a05-120">顧客に対してアクセス許可を有効にすると、顧客は独自のリソース (Azure の予約の購入など) を購入できるようになります。</span><span class="sxs-lookup"><span data-stu-id="53a05-120">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="53a05-121">パートナーセンターにおける顧客のアクセス許可の概要</span><span class="sxs-lookup"><span data-stu-id="53a05-121">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="53a05-122">[顧客**アカウント**] ページを使用して、顧客のアクセス許可をオンまたはオフにします。</span><span class="sxs-lookup"><span data-stu-id="53a05-122">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="53a05-123">現在、この機能は以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="53a05-123">Currently, this feature supports:</span></span>

- <span data-ttu-id="53a05-124">**Azure の予約:** このアクセス許可を有効にすると、顧客は、購入した特定の Azure サブスクリプションに対して独自の Azure 予約を購入できます。</span><span class="sxs-lookup"><span data-stu-id="53a05-124">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="53a05-125">カスタマーアクセス許可を有効にする前に、次の重要な点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="53a05-125">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="53a05-126">既定では、顧客のアクセス許可は、パートナーセンターで自動的に無効 (オフ) になります。</span><span class="sxs-lookup"><span data-stu-id="53a05-126">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>
- <span data-ttu-id="53a05-127">顧客に対するアクセス許可をオンまたはオフにする前に、パートナーセンターの管理エージェントの役割が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="53a05-127">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>
  <span data-ttu-id="53a05-128">販売代理店またはヘルプデスクエージェントの役割が割り当てられているパートナーには、読み取り専用のアクセス権があり、顧客のアクセス許可をオンまたはオフにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="53a05-128">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>
- <span data-ttu-id="53a05-129">選択した顧客に対してアクセス許可を有効にする (有効にする) ことができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-129">You can turn on (enable) permissions for any customer you choose.</span></span>
- <span data-ttu-id="53a05-130">パートナーセンターのダッシュボードまたは[パートナーセンター api](https://docs.microsoft.com/partner-center/develop/manage-customers)を使用して、顧客のアクセス許可をオンまたはオフにすることができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-130">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>
- <span data-ttu-id="53a05-131">特定の顧客に対して [(有効)] アクセス許可を有効にした後、その顧客によるその後の購入については、支払いが行われます。</span><span class="sxs-lookup"><span data-stu-id="53a05-131">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="53a05-132">お客様が購入を交換、取り消し、または更新する場合は、自分で購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="53a05-132">If customers want to exchange, cancel or renew a purchase they have made, they will not be able to do so themselves.</span></span> <span data-ttu-id="53a05-133">パートナーは、これらの購入を交換、キャンセル、または更新するために、パートナーとして依頼する必要があります。</span><span class="sxs-lookup"><span data-stu-id="53a05-133">They need to ask you, as the partner, to help them exchange, cancel, or renew these purchases.</span></span>
- <span data-ttu-id="53a05-134">特定の顧客に対してアクセス許可を有効にした後は、顧客がそれ以降に購入したことは通知**されません**。</span><span class="sxs-lookup"><span data-stu-id="53a05-134">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>
- <span data-ttu-id="53a05-135">顧客によるその後の購入は、お客様が行った購入と共にパートナーセンターに表示されます。</span><span class="sxs-lookup"><span data-stu-id="53a05-135">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="53a05-136">これらの購入は、顧客の**注文履歴**ページ、**予約**ページ、または[**アクティビティログ**](activity-logs.md)で見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-136">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="53a05-137">独自の Azure 予約を購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="53a05-137">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="53a05-138">Azure の予約は、割引料金で Azure サービスを購入するための優れた方法です。</span><span class="sxs-lookup"><span data-stu-id="53a05-138">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="53a05-139">Azure の予約の利点の詳細については、「 [Azure Reservations とは](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53a05-139">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="53a05-140">これで、お客様に代わって Azure の予約を購入することができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-140">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="53a05-141">または、自分の Azure 予約を購入するためのアクセス許可を顧客に与えることができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-141">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="53a05-142">お客様に独自の Azure 予約を購入するアクセス許可を付与した後、購入した予約を管理する方法を理解するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="53a05-142">After you give customers permission to buy their own Azure reservations, you can help them understand how to manage any reservations they purchase.</span></span> <span data-ttu-id="53a05-143">たとえば、予約の使用を最適化する方法や、予約のスコープを変更する方法をお客様が知りたい場合があります。</span><span class="sxs-lookup"><span data-stu-id="53a05-143">For instance, customers might want to know how to optimize their use of a reservation or how to change a reservation’s scope.</span></span> <span data-ttu-id="53a05-144">これらのトピックの詳細については、「 [Azure リソースの予約を管理]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance)する」をお読みください。</span><span class="sxs-lookup"><span data-stu-id="53a05-144">For more information about these topics, ask customers to read [Manage reservations for Azure resources]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="53a05-145">顧客が独自の Azure 予約を購入できるようにするには</span><span class="sxs-lookup"><span data-stu-id="53a05-145">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="53a05-146">顧客に代わって購入した既存の Azure プランまたは Azure グローバルサブスクリプションがあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="53a05-146">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="53a05-147">お客様にこのサブスクリプションの**所有者**ロールが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="53a05-147">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="53a05-148">自分の Azure 予約を購入するには、顧客のアクセス許可を有効にします (こ**の機能を**有効にします)。</span><span class="sxs-lookup"><span data-stu-id="53a05-148">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="53a05-149">各手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="53a05-149">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="53a05-150">顧客が既存の Azure サブスクリプションを持っていることを確認する</span><span class="sxs-lookup"><span data-stu-id="53a05-150">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="53a05-151">顧客に独自の Azure 予約を購入するアクセス許可を付与する前に、顧客が既存の Azure プランまたは Azure グローバルサブスクリプションを持っていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="53a05-151">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="53a05-152">顧客がパートナーセンターで現在の Azure サブスクリプションを表示していない場合は、顧客のアクセス許可を有効にする前にサブスクリプションを購入する必要があります。</span><span class="sxs-lookup"><span data-stu-id="53a05-152">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="53a05-153">顧客が既に Azure サブスクリプションを持っているかどうかを確認するには、パートナーセンターのダッシュボードにサインインし、[ **CSP** ]、[**顧客**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-153">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="53a05-154">一覧から特定の顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-154">Select the specific customer from the list.</span></span> <span data-ttu-id="53a05-155">次に、[**サブスクリプション**] を選択し、azure プランまたは azure グローバルのいずれかの使用量ベースのサブスクリプションを検索します。</span><span class="sxs-lookup"><span data-stu-id="53a05-155">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="53a05-156">顧客が既存の Azure サブスクリプションを持っていない場合は、サブスクリプションを購入することができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-156">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="53a05-157">「 [Azure プランの購入」を](purchase-azure-plan.md)参照してください。</span><span class="sxs-lookup"><span data-stu-id="53a05-157">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="53a05-158">お客様に Azure の正しいロールが割り当てられていることを確認する</span><span class="sxs-lookup"><span data-stu-id="53a05-158">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="53a05-159">顧客が既存の Azure サブスクリプションを持っていることを確認した後、顧客に関連付けられているキーユーザーに、その Azure サブスクリプションの正しい**所有者**ロールが割り当てられていることを確認する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="53a05-159">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="53a05-160">これは、お客様が購入した Azure サブスクリプションの Azure 予約を購入する必要がある、ロールベースのアクセス (RBAC) です。</span><span class="sxs-lookup"><span data-stu-id="53a05-160">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="53a05-161">パートナーによっては、自分の Azure リソースを積極的に管理およびプロビジョニングすることを希望するお客様に、既に**所有者**ロールが割り当てられている場合があります。</span><span class="sxs-lookup"><span data-stu-id="53a05-161">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="53a05-162">以前に購入したサブスクリプションを管理するために、既に**所有者**の状態を顧客に割り当てている場合は、この手順を省略できます。</span><span class="sxs-lookup"><span data-stu-id="53a05-162">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="53a05-163">**所有者**ロールが割り当てられていない場合、ユーザーは Azure の予約を購入できないように Azure portal にエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="53a05-163">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="53a05-164">顧客に Azure サブスクリプションの**所有者**ロールが割り当てられていることを確認するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="53a05-164">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="53a05-165">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="53a05-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="53a05-166">[ **CSP**]、[**顧客**] の順に選択し、特定の顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-166">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="53a05-167">その顧客の**サブスクリプション**を選択し、特定の Azure サブスクリプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="53a05-167">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="53a05-168">その顧客のサブスクリプションの横にある [**管理**] ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-168">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="53a05-169">これにより、 [Azure portal](https://portal.azure.com/)が開きます。</span><span class="sxs-lookup"><span data-stu-id="53a05-169">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="53a05-170">特定のユーザーに**所有者**ロールを割り当てるには、次の手順に従っ[て、管理者としてユーザーを割り当て](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)ます。</span><span class="sxs-lookup"><span data-stu-id="53a05-170">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="53a05-171">独自の Azure 予約を購入するには、顧客のアクセス許可をオンまたはオフにします</span><span class="sxs-lookup"><span data-stu-id="53a05-171">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="53a05-172">顧客に既存の Azure サブスクリプションがあることを確認し、ユーザーにそのサブスクリプションの**所有者**ロールが割り当てられていることを確認したら、顧客のアクセス許可を有効にする (有効にする) ことができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-172">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="53a05-173">また、これらの手順を使用して、顧客のアクセス許可をオフ (無効) にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="53a05-173">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="53a05-174">パートナーセンターのダッシュボードまたは[パートナーセンター api](https://docs.microsoft.com/partner-center/develop/manage-customers)を使用して、顧客のアクセス許可を有効または無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="53a05-174">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="53a05-175">パートナーセンターで顧客のアクセス許可をオンまたはオフにするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="53a05-175">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="53a05-176">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="53a05-176">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="53a05-177">左側のナビゲーションメニューで、[ **CSP**]、[ **Customers**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-177">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="53a05-178">顧客リストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="53a05-178">A customer list appears.</span></span>

3. <span data-ttu-id="53a05-179">特定の顧客名を選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-179">Select a specific customer name.</span></span>

4. <span data-ttu-id="53a05-180">[Customer] メニューから [ **Account** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="53a05-180">Select **Account** from the customer menu.</span></span> <span data-ttu-id="53a05-181">[顧客**アカウント**] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="53a05-181">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="53a05-182">ページの下部にある [**顧客のアクセス許可**] 領域を探します。</span><span class="sxs-lookup"><span data-stu-id="53a05-182">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   ![アカウントページに対する顧客のアクセス許可](images/give-customers-permission-reservations.png)

6. <span data-ttu-id="53a05-184">[ **Azure の予約**] で、[**顧客の購入を許可する**] オプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="53a05-184">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="53a05-185">顧客のアクセス許可を有効にするには、このオプションの横にあるスイッチを**on**の位置に移動します。</span><span class="sxs-lookup"><span data-stu-id="53a05-185">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="53a05-186">顧客のアクセス許可を無効にするには、スイッチを**off**の位置に移動します。</span><span class="sxs-lookup"><span data-stu-id="53a05-186">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="53a05-187">お客様の Azure 予約を購入するために顧客のアクセス許可を有効にした場合に何が起こるかについては、「[パートナーセンターにおける顧客のアクセス許可の概要](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53a05-187">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span> <span data-ttu-id="53a05-188">カスタマーアクセス許可をオンまたはオフにすると、アクティビティログに各アクションが記録されます。</span><span class="sxs-lookup"><span data-stu-id="53a05-188">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="53a05-189">(パートナーセンターのダッシュボードの上部にある歯車アイコンを選択すると、このログにアクセスできます)。</span><span class="sxs-lookup"><span data-stu-id="53a05-189">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="53a05-190">顧客のアクセス許可をオンまたはオフにすると、アクティビティログで [**顧客の購入のアクセス許可を作成**] または [顧客の購入の**アクセス許可を削除**する] のいずれかの操作が表示されます。</span><span class="sxs-lookup"><span data-stu-id="53a05-190">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="see-also"></a><span data-ttu-id="53a05-191">関連項目</span><span class="sxs-lookup"><span data-stu-id="53a05-191">See also</span></span>

- [<span data-ttu-id="53a05-192">顧客に代わって Azure の予約を購入する</span><span class="sxs-lookup"><span data-stu-id="53a05-192">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="53a05-193">パートナーセンター-Microsoft 予約の販売</span><span class="sxs-lookup"><span data-stu-id="53a05-193">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)
- [<span data-ttu-id="53a05-194">顧客に代わって Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="53a05-194">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md) 