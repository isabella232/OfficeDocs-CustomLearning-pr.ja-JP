---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学習経路のトラブルシューティング
ms.date: 02/10/2019
description: Microsoft 365 ラーニング パスのトラブルシューティング方法について説明します。
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000303"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="c5731-103">Microsoft 365 ラーニング パスのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="c5731-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="c5731-104">Microsoft 365 ラーニング パスまたは SharePoint Online プロビジョニング サービスで発生する可能性がある問題のトラブルシューティングのヒントを次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5731-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="c5731-105">テナント管理者のアクセス許可を持っているかどうかの確認方法</span><span class="sxs-lookup"><span data-stu-id="c5731-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="c5731-106">SharePoint Online Provisioning Service にサインインし、カスタム 学習をプロビジョニングするには、テナント管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5731-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="c5731-107">SharePoint Online Provisioning Service でサインインに関する問題が発生している場合は、グローバル管理者の役割が割り当てられていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c5731-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="c5731-108">カスタム 学習ソリューションには、テナント管理者のアクセス許可 (365 グローバル管理者Officeと呼ばれる) が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5731-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="c5731-109">グローバル管理者の役割が割り当てられているかどうかを確認する方法を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5731-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="c5731-110">サインインして Office.com。</span><span class="sxs-lookup"><span data-stu-id="c5731-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="c5731-111">[管理者 **] をクリックします。**</span><span class="sxs-lookup"><span data-stu-id="c5731-111">Click **Admin**</span></span>
3.  <span data-ttu-id="c5731-112">[ユーザー **] で**、[アクティブな **ユーザー] を選択します。**</span><span class="sxs-lookup"><span data-stu-id="c5731-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="c5731-113">名前を検索する</span><span class="sxs-lookup"><span data-stu-id="c5731-113">Search for your name</span></span>
5.  <span data-ttu-id="c5731-114">[検索結果] で自分の名前をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c5731-114">Click your name in Search results.</span></span> <span data-ttu-id="c5731-115">役割のグローバル管理者が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c5731-115">You should see Global administrator for your role.</span></span>
<span data-ttu-id="c5731-116">![ライセンス、グループ メンバーシップ、その他の情報と共に役割を一覧表示するサンプル ページ。](media/cg-globaladminrole.png)</span><span class="sxs-lookup"><span data-stu-id="c5731-116">![Sample page that lists your role along with licenses, group memberships and other information.](media/cg-globaladminrole.png)</span></span>

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="c5731-117">グローバル管理者の役割を持ってない場合</span><span class="sxs-lookup"><span data-stu-id="c5731-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="c5731-118">組織でグローバル管理者を見つけて、そのユーザーにサービスにサインインするか、グローバル管理者の役割を割り当てします。</span><span class="sxs-lookup"><span data-stu-id="c5731-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="c5731-119">テナント アプリ カタログのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="c5731-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="c5731-120">カスタム学習では、ターゲット テナントにアプリ カタログをプロビジョニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="c5731-121">アプリ カタログを作成するには、グローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5731-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="c5731-122">アプリ カタログに関する一般的な問題のトラブルシューティング手順を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5731-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="c5731-123">テナント アプリ カタログを持っているかどうかの確認方法</span><span class="sxs-lookup"><span data-stu-id="c5731-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="c5731-124">まず、グローバル管理者のアクセス許可を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="c5731-125">上記の「テナント管理者のアクセス許可」の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5731-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="c5731-126">[Office 365 から、[**管理**] をクリックし、[展開] 矢印をクリック>、[すべての管理センター SharePoint を表示する]  >    >  **をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c5731-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="c5731-127">[**従来の管理 SharePoint Center アプリ**  >  **アプリ**  >  **カタログ] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c5731-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="c5731-128">[ **アプリ] の** 下に、[SharePoint 用アプリの配布 **] というタイトルのタイルが表示されます**。</span><span class="sxs-lookup"><span data-stu-id="c5731-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="c5731-129">タイルが表示される場合は、テナント アプリ カタログがあります。</span><span class="sxs-lookup"><span data-stu-id="c5731-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="c5731-130">以下の **「サイト の Colllection...」** セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5731-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="c5731-131">タイルが表示されていない場合は、テナント用のテナント アプリ カタログを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="c5731-132">以下の「 **テナント アプリ カタログを作成する方法」** セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5731-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="c5731-133">テナント アプリ カタログのサイト コレクション所有者を確認する方法</span><span class="sxs-lookup"><span data-stu-id="c5731-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="c5731-134">Microsoft 365 ラーニング パスをプロビジョニングするには、テナント アプリ カタログのサイト コレクション所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="c5731-135">所有者かどうかを確認する方法を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5731-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="c5731-136">[Office 365 から、[**管理**] をクリックし、[展開] 矢印をクリック>、[すべての管理センター SharePoint を表示する]  >    >  **をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c5731-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="c5731-137">[ **クラシック管理 SharePoint センター] をクリック** し、アプリ カタログ **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="c5731-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="c5731-138">[ **所有者] を** 選択し、サイト コレクションの所有者を確認します。</span><span class="sxs-lookup"><span data-stu-id="c5731-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="c5731-139">これは次のように見える必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-139">It should look something like this.</span></span>
<span data-ttu-id="c5731-140">![[管理者の管理] ページ。](media/cg-sitecollectionowner.png)</span><span class="sxs-lookup"><span data-stu-id="c5731-140">![Manage administrators page.](media/cg-sitecollectionowner.png)</span></span>

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="c5731-141">テナント アプリ カタログが存在しない場合の作成方法</span><span class="sxs-lookup"><span data-stu-id="c5731-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="c5731-142">SharePoint Online 管理者Office 365 にサインインします。</span><span class="sxs-lookup"><span data-stu-id="c5731-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="c5731-143">**[管理者]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c5731-143">Click **Admin**.</span></span>
3. <span data-ttu-id="c5731-144">[管理 **センター] で\*\*\*\*、[SharePoint] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c5731-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="c5731-145">[アプリ **アプリ**  >  **カタログ] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c5731-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="c5731-146">[新 **しいアプリ カタログ サイトの作成] をクリック** し **、[OK] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c5731-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="c5731-147">アプリ カタログの情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="c5731-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="c5731-148">複数の管理者を含める場合があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="c5731-149">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="c5731-149">The following shows an example.</span></span>  
![新しいアプリ カタログの情報を入力するフォーム。](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="c5731-151">これで完了です。</span><span class="sxs-lookup"><span data-stu-id="c5731-151">That’s it.</span></span> <span data-ttu-id="c5731-152">完了です。</span><span class="sxs-lookup"><span data-stu-id="c5731-152">You’re done.</span></span> <span data-ttu-id="c5731-153">ただし、カスタム 学習のプロビジョニングに移行する前に、アプリ カタログの作成が完了するまで少なくとも 30 分待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5731-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="c5731-154">カスタム学習をプロビジョニングする前に、テナント アプリ カタログを作成してから少なくとも 30 分待ちます。</span><span class="sxs-lookup"><span data-stu-id="c5731-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="c5731-155">これにより、SharePoint 内でアプリ カタログのプロビジョニング プロセスが完了します。</span><span class="sxs-lookup"><span data-stu-id="c5731-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 