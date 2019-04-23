---
author: pkrebs
ms.author: pkrebs
title: カスタム学習 Office 365 サイトに移動する
ms.date: 02/18/2019
description: カスタム学習サイトに移動する
ms.openlocfilehash: 220d27d6f12f4edb26e0d46ac76cbcea12270e74
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055804"
---
# <a name="add-owners-custom-learning-site"></a><span data-ttu-id="1d98c-103">所有者の追加カスタム学習サイト</span><span class="sxs-lookup"><span data-stu-id="1d98c-103">Add Owners Custom Learning site</span></span>

<span data-ttu-id="1d98c-104">office 365 サイト用のカスタム学習サイトは office 365 テナントでホストされているので、まだサインインしていない場合は、office 365 にサインインしてサイトにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d98c-104">The Custom Learning for Office 365 site is hosted in your Office 365 tenant, so you'll need to sign in to Office 365, if you're not already signed in, to get to the site.</span></span> 

## <a name="sign-in-to-office-365"></a><span data-ttu-id="1d98c-105">Office 365 にサインインする</span><span class="sxs-lookup"><span data-stu-id="1d98c-105">Sign in to Office 365</span></span> 

1.  <span data-ttu-id="1d98c-106">Web ブラウザーを開き、office.com または組織のサインインの場所に移動します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-106">Open your Web browser and navigate to office.com or your organization’s sign-in location.</span></span> 
2.  <span data-ttu-id="1d98c-107">ユーザー名とパスワードを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="1d98c-107">Sign in with your user name and password.</span></span>
3.  <span data-ttu-id="1d98c-108">サイトの場所に移動します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-108">Navigate to the location of the site.</span></span> <span data-ttu-id="1d98c-109">使用可能な状態になっていない場合は、PnP プロビジョニングサービスから受信したメールで見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="1d98c-109">If you don't have it available, you can find it in the mail you recieved from the PnP Provisioning Service.</span></span> <span data-ttu-id="1d98c-110">office 365 ホームページから [SharePoint] を選択し、[ **office 365 サイト用のカスタム学習**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-110">Select SharePoint from the Office 365 Home page, and then select the **Custom Learning for Office 365** site.</span></span> <span data-ttu-id="1d98c-111">別の名前を付けることができます。</span><span class="sxs-lookup"><span data-stu-id="1d98c-111">You may have named it different.</span></span> 
5. <span data-ttu-id="1d98c-112">**Office 365 のトレーニング**タイルをクリックして、カスタム学習で利用可能な完全なトレーニングプレイリストを表示し、カスタム学習が期待どおりに動作することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-112">Click the **Office 365 training** tile to see the full suite of training playlist available with Custom Learning and to verify Custom Learning is working as expected.</span></span> 

![cg-goto](media/cg-goto.png)

## <a name="view-all-the-custom-learning-content"></a><span data-ttu-id="1d98c-114">すべてのカスタム学習コンテンツを表示する</span><span class="sxs-lookup"><span data-stu-id="1d98c-114">View all the Custom Learning content</span></span>
<span data-ttu-id="1d98c-115">Office 365 トレーニングページでは、カスタム学習用に使用可能なすべてのトレーニングを表示するように構成されたカスタム学習 Web パーツをホストしています。</span><span class="sxs-lookup"><span data-stu-id="1d98c-115">The Office 365 training page hosts the Custom Learning Web part configured to show all the training available for Custom Learning.</span></span> 

1. <span data-ttu-id="1d98c-116">ページを下にスクロールして、すべてのカテゴリとサブカテゴリを表示します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-116">Scroll down the page to view all the categories and subcategories.</span></span>
2. <span data-ttu-id="1d98c-117">タイヤを少し開始します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-117">Kick the tires a bit.</span></span> <span data-ttu-id="1d98c-118">いくつかのサブカテゴリをクリックしてから、いくつかの再生リストをクリックして、カスタム学習コンテンツの編成方法を把握します。</span><span class="sxs-lookup"><span data-stu-id="1d98c-118">Click a few subcategories, and then click a few playlists to get a feel for how Custom Learning content is organized.</span></span> 

![cg-gotoall](media/cg-gotoall.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="1d98c-120">サイトに所有者を追加する</span><span class="sxs-lookup"><span data-stu-id="1d98c-120">Add Owners to Site</span></span>
<span data-ttu-id="1d98c-121">テナント管理者は、サイトをカスタマイズするユーザーになる可能性があるので、サイトにいくつかの所有者を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d98c-121">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="1d98c-122">所有者はサイトの管理権限を持っているため、サイトのページを変更したり、サイトを再ブランド化したりできます。</span><span class="sxs-lookup"><span data-stu-id="1d98c-122">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="1d98c-123">また、カスタム学習 Web パーツを通じて配信されるコンテンツを非表示にしたり、表示したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="1d98c-123">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="1d98c-124">また、カスタムのプレイリストを作成してカスタムサブカテゴリに割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="1d98c-124">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="1d98c-125">[SharePoint の**設定**] メニューの [**サイトの権限**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1d98c-125">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="1d98c-126">[**高度なアクセス許可の設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1d98c-126">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="1d98c-127">[ **Office 365 所有者向けのカスタム学習] を**クリックします。</span><span class="sxs-lookup"><span data-stu-id="1d98c-127">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="1d98c-128">[**新しい** > **ユーザーをこのグループに追加する**] をクリックし、所有者にするユーザーを追加して、[**共有**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1d98c-128">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

