---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学習経路のトラブルシューティング
ms.date: 02/10/2019
description: Microsoft 365 学習経路のトラブルシューティング方法について説明します。
ms.service: sharepoint online
ms.openlocfilehash: 8d8b418c7a4b2c025391eb4527af86b02738c532
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233869"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="ce2c1-103">Microsoft 365 学習経路のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ce2c1-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="ce2c1-104">ここでは、Microsoft 365 の学習経路または SharePoint Online プロビジョニングサービスで発生する可能性のある問題のトラブルシューティングのヒントを示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="ce2c1-105">テナント管理者のアクセス許可があるかどうかを確認する方法</span><span class="sxs-lookup"><span data-stu-id="ce2c1-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="ce2c1-106">SharePoint Online プロビジョニングサービスにサインインし、カスタム学習を準備するには、テナント管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="ce2c1-107">SharePoint Online プロビジョニングサービスでサインインに関する問題が発生している場合は、全体管理者の役割が割り当てられていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="ce2c1-108">カスタム学習ソリューションには、テナント管理者のアクセス許可が必要です。それ以外の場合は、Office 365 のグローバル管理者ロールと呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="ce2c1-109">グローバル管理者の役割が割り当てられているかどうかを確認する方法は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="ce2c1-110">Office.com にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="ce2c1-111">[**管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-111">Click **Admin**</span></span>
3.  <span data-ttu-id="ce2c1-112">[**ユーザー**] で、[**アクティブなユーザー** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="ce2c1-113">自分の名前を検索する</span><span class="sxs-lookup"><span data-stu-id="ce2c1-113">Search for your name</span></span>
5.  <span data-ttu-id="ce2c1-114">[検索結果] で自分の名前をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-114">Click your name in Search results.</span></span> <span data-ttu-id="ce2c1-115">役割の全体管理者が表示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-115">You should see Global administrator for your role.</span></span>

![cg-globaladminrole.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="ce2c1-117">グローバル管理者の役割を持っていない場合</span><span class="sxs-lookup"><span data-stu-id="ce2c1-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="ce2c1-118">組織内のグローバル管理者を検索して、そのユーザーがサービスにサインインしたり、グローバル管理者の役割を割り当てたりするようにします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="ce2c1-119">テナントのアプリカタログのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ce2c1-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="ce2c1-120">カスタム学習では、ターゲットテナントにアプリカタログをプロビジョニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="ce2c1-121">アプリカタログを作成するには、グローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="ce2c1-122">一般的なアプリカタログの問題のトラブルシューティング手順を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="ce2c1-123">テナントアプリカタログがあるかどうかを確認する方法</span><span class="sxs-lookup"><span data-stu-id="ce2c1-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="ce2c1-124">手始めとして、全体管理者のアクセス許可があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="ce2c1-125">前述のテナント管理者権限の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="ce2c1-126">Office 365 で、[**管理者**] をクリックし > [展開] の矢印をクリックし、[すべての**Show all**  >  **管理センター**  >  の**SharePoint**を表示] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="ce2c1-127">[**従来の管理者 SharePoint センター**  >  **アプリ**  >  の**アプリカタログ**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="ce2c1-128">[ **アプリ**] の下に、[ **SharePoint 用アプリの配布**] というタイトルのタイルが表示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="ce2c1-129">タイルが表示されている場合は、テナントのアプリカタログがあります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="ce2c1-130">下記の「サイトの詳細を **確認する方法** 」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="ce2c1-131">タイルが表示されない場合は、テナントのテナントアプリカタログを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="ce2c1-132">「 **How to create a Tenant App Catalog** 」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="ce2c1-133">テナントアプリカタログのサイトコレクションの所有者であることを確認する方法</span><span class="sxs-lookup"><span data-stu-id="ce2c1-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="ce2c1-134">Microsoft 365 learning の経路をプロビジョニングするには、テナントのアプリカタログのサイトコレクションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="ce2c1-135">所有者であるかどうかを判断する方法は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="ce2c1-136">Office 365 で、[**管理者**] をクリックし > [展開] の矢印をクリックし、[すべての**Show all**  >  **管理センター**  >  の**SharePoint**を表示] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="ce2c1-137">[ **従来の管理者 SharePoint センター**] をクリックし、 **アプリカタログ**を選択します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="ce2c1-138">[ **所有者**] を選択し、サイトコレクションの所有者であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="ce2c1-139">これは次のようなものになります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-139">It should look something like this.</span></span>
 
![cg-sitecollectionowner.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="ce2c1-141">テナントのアプリカタログを作成する方法 (存在しない場合)</span><span class="sxs-lookup"><span data-stu-id="ce2c1-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="ce2c1-142">SharePoint Online 管理者アカウントを使用して、Office 365 にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="ce2c1-143">**[管理者]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-143">Click **Admin**.</span></span>
3. <span data-ttu-id="ce2c1-144">[ **管理センター**] で、[ **SharePoint**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="ce2c1-145">[**アプリ**  >  **アプリカタログ**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="ce2c1-146">[ **新しいアプリカタログサイトを作成する**] をクリックし、[ **OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="ce2c1-147">アプリカタログの情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="ce2c1-148">複数の管理者を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="ce2c1-149">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-149">The following shows an example.</span></span>  

![cg-appcatalogfinish.png](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="ce2c1-151">これで完了です。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-151">That’s it.</span></span> <span data-ttu-id="ce2c1-152">完了しました。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-152">You’re done.</span></span> <span data-ttu-id="ce2c1-153">ただし、カスタム学習のプロビジョニングに移行する前に、アプリカタログの作成が完了したことを確認するために、少なくとも30分待機する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ce2c1-154">テナントのアプリカタログを作成した後、少なくとも30分待ってから、カスタム学習をプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="ce2c1-155">これにより、アプリカタログのプロビジョニングプロセスが SharePoint 内で完了するようになります。</span><span class="sxs-lookup"><span data-stu-id="ce2c1-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 