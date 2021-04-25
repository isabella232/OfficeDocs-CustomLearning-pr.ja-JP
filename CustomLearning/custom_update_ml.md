---
author: pkrebs
ms.author: pkrebs
title: 多言語サポートの学習経路を更新する
ms.date: 05/20/2019
description: 多言語サポートの学習経路を更新する
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 9344cd91e5b6718b1eb0e73e25fdc8311afed793
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000243"
---
# <a name="update-learning-pathways-for-multilingual-support"></a><span data-ttu-id="421b9-103">多言語サポートの学習経路を更新する</span><span class="sxs-lookup"><span data-stu-id="421b9-103">Update learning pathways for multilingual support</span></span>
<span data-ttu-id="421b9-104">既存のラーニング パスウェイ サイトがある場合は、多言語サポート用に更新できます。</span><span class="sxs-lookup"><span data-stu-id="421b9-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="421b9-105">多言語 4.0 バージョンへの学習パスを更新するには、Web パーツ パッケージ customlearning.sppkg を SharePoint テナント アプリ カタログにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="421b9-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="421b9-106">学習経路を更新する場合:</span><span class="sxs-lookup"><span data-stu-id="421b9-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="421b9-107">以前に作成されたカスタムプレイリストとアセットは維持されます</span><span class="sxs-lookup"><span data-stu-id="421b9-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="421b9-108">コンテンツを非表示または表示する設定が維持される</span><span class="sxs-lookup"><span data-stu-id="421b9-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="421b9-109">SharePoint テンプレートの学習経路は変更されません</span><span class="sxs-lookup"><span data-stu-id="421b9-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="421b9-110">学習経路サイト ページは翻訳されません。</span><span class="sxs-lookup"><span data-stu-id="421b9-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="421b9-111">この作業は手動で行う必要があります</span><span class="sxs-lookup"><span data-stu-id="421b9-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="421b9-112">多言語の学習経路の概要を読む</span><span class="sxs-lookup"><span data-stu-id="421b9-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="421b9-113">多言語サポートが学習経路でどのように機能するのかについては、「ラーニング パス多言語の [概要」をご覧ください](custom_overview_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="421b9-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview_ml.md)).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="421b9-114">更新の前提条件</span><span class="sxs-lookup"><span data-stu-id="421b9-114">Prerequisites to update</span></span>
<span data-ttu-id="421b9-115">学習経路を更新する前に、次の前提条件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="421b9-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="421b9-116">ラーニング パスを更新するユーザーは、テナント アプリ カタログのサイト コレクション所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="421b9-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="421b9-117">ユーザープロビジョニング学習パスがアプリ カタログのサイト コレクション所有者ではない場合は、次の手順 [を実行](addappadmin.md) して続行します。</span><span class="sxs-lookup"><span data-stu-id="421b9-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="421b9-118">言語設定の設定</span><span class="sxs-lookup"><span data-stu-id="421b9-118">Set language settings</span></span> 
<span data-ttu-id="421b9-119">学習経路を更新する前に、サイトの言語設定を設定します。</span><span class="sxs-lookup"><span data-stu-id="421b9-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="421b9-120">ラーニング パス サイトの多言語サポートを有効にするには、[ページとニュースを複数の言語に翻訳するを有効にする] を **[オン**] に設定し、サイトでサポートする言語を追加できます。</span><span class="sxs-lookup"><span data-stu-id="421b9-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="421b9-121">ラーニング パスサイトで、右 **から [設定** ] を選択し、[サイト情報] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="421b9-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="421b9-122">サイト情報ウィンドウの下部で、[すべてのサイト設定を表示 **する] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="421b9-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="421b9-123">[サイト **の管理] で**、[言語の **設定] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="421b9-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="421b9-124">[ **複数の言語に翻訳する** ページとニュースを有効にする] で、トグル スイッチを設定します。</span><span class="sxs-lookup"><span data-stu-id="421b9-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="421b9-125">複数のサイトの場合は、トグルを **[オン**] にスライドし、[言語の追加] セクションに進みます。</span><span class="sxs-lookup"><span data-stu-id="421b9-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="421b9-126">英語専用サイトの場合は、トグルを Off にスライド **します**。</span><span class="sxs-lookup"><span data-stu-id="421b9-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="421b9-127">言語を追加する</span><span class="sxs-lookup"><span data-stu-id="421b9-127">Add languages</span></span>
<span data-ttu-id="421b9-128">学習経路は 9 つの言語をサポートします。必要な言語のみを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="421b9-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="421b9-129">このドキュメントで使用されている例では、イタリア語が追加されます。</span><span class="sxs-lookup"><span data-stu-id="421b9-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="421b9-130">[**サイト言語の追加と** 削除] で、[言語の選択または入力] で言語名の入力を開始するか、ドロップダウンから言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="421b9-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="421b9-131">この手順を繰り返して、複数の言語を追加できます。</span><span class="sxs-lookup"><span data-stu-id="421b9-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="421b9-132">このページに戻って、いつでもサイトの言語を追加または削除できます。</span><span class="sxs-lookup"><span data-stu-id="421b9-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="421b9-133">翻訳者の割り当て</span><span class="sxs-lookup"><span data-stu-id="421b9-133">Assign translators</span></span>
<span data-ttu-id="421b9-134">学習経路の言語設定を定義する場合は、翻訳者を割り当てできます。</span><span class="sxs-lookup"><span data-stu-id="421b9-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="421b9-135">翻訳者には外国語プロファイルが設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="421b9-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="421b9-136">外国語プロファイルの詳細については、「多言語コミュニケーション サイト、ページ、ニュースを作成する [」を参照してください](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。</span><span class="sxs-lookup"><span data-stu-id="421b9-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="421b9-137">サポートされている言語の場合は、[選択] **をクリックするか、翻訳者を入力** し、翻訳者を選択します。</span><span class="sxs-lookup"><span data-stu-id="421b9-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="421b9-138">ラーニング パス Web パーツ パッケージを更新する</span><span class="sxs-lookup"><span data-stu-id="421b9-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="421b9-139">この手順では、学習パス 4.0 Web パーツを SharePoint アプリ カタログにアップロードし、[ラーニング パス管理] ページに移動して更新プロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="421b9-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="421b9-140">Web パーツ パッケージのアップロード</span><span class="sxs-lookup"><span data-stu-id="421b9-140">Upload the web part package</span></span>
1.  <span data-ttu-id="421b9-141">[GitHub カスタム学習リポジトリに移動](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)し **、customlearning.sppkg** を選択し、PC 上のローカル ドライブにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="421b9-141">Go to the [GitHub custom learning repository](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), select **customlearning.sppkg** and then download it to a local drive on your PC.</span></span> 
2.  <span data-ttu-id="421b9-142">まだサインインしていない場合は、テナント管理者またはサイト コレクション管理者アカウントを使用して、テナントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="421b9-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="421b9-143">[管理 **] [**  >  すべての SharePoint **の**  >  **その他の**  >  **機能を表示する] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="421b9-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="421b9-144">[アプリ **] で**、[開く] **をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="421b9-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="421b9-145">[SharePoint **用**  >  **アプリ カタログ配布アプリ] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="421b9-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="421b9-146">[ファイル **のアップロード**  >  **] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="421b9-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="421b9-147">ダウンロードした **customlearning.sppkg** ファイルを選択し **、[OK** 展開] を  >  **クリックします**。</span><span class="sxs-lookup"><span data-stu-id="421b9-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="421b9-148">更新プログラムを完了する</span><span class="sxs-lookup"><span data-stu-id="421b9-148">Complete the update</span></span>
1.  <span data-ttu-id="421b9-149">[ラーニング パス] サイトで、[ホーム] メニューから [ラーニング **パスの管理** ] **を選択** します。</span><span class="sxs-lookup"><span data-stu-id="421b9-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="421b9-150">更新を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="421b9-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="421b9-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="421b9-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="421b9-152">**[開始]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="421b9-152">Click **Start**.</span></span> 
4. <span data-ttu-id="421b9-153">更新が完了したら、[閉じる] を **クリックします**。</span><span class="sxs-lookup"><span data-stu-id="421b9-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="421b9-154">次の手順</span><span class="sxs-lookup"><span data-stu-id="421b9-154">Next Steps</span></span>
- <span data-ttu-id="421b9-155">サイトと [Web パーツで提供](custom_exploresite.md) される既定のコンテンツを確認します。</span><span class="sxs-lookup"><span data-stu-id="421b9-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="421b9-156">サイト ページの翻訳の詳細については、「サイト ページの翻訳 [」を参照してください](custom_translate_page_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="421b9-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

