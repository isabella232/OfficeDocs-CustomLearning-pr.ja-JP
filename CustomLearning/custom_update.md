---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学習経路をアップデートする
ms.date: 07/06/2020
description: Microsoft 365 学習経路をアップデートする
ms.service: sharepoint online
ms.openlocfilehash: 3f1874849832224726e452912c9228411ecd0820
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233849"
---
# <a name="update-learning-pathways"></a><span data-ttu-id="908f3-103">学習経路を更新する</span><span class="sxs-lookup"><span data-stu-id="908f3-103">Update learning pathways</span></span>
<span data-ttu-id="908f3-104">既存のラーニングパスサイトがある場合は、多言語サポートのために更新できます。</span><span class="sxs-lookup"><span data-stu-id="908f3-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="908f3-105">マルチリンガル4.0 バージョンへの学習経路を更新するには、web パーツパッケージ customlearning を SharePoint テナントアプリカタログにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="908f3-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="908f3-106">学習経路を更新すると、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="908f3-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="908f3-107">以前に作成したカスタムの再生リストとアセットは保持されます。</span><span class="sxs-lookup"><span data-stu-id="908f3-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="908f3-108">コンテンツの表示/非表示の設定は維持されます。</span><span class="sxs-lookup"><span data-stu-id="908f3-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="908f3-109">ラーニング経路 SharePoint テンプレートは未変更のままです。</span><span class="sxs-lookup"><span data-stu-id="908f3-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="908f3-110">ラーニングパスサイトページは変換されません。</span><span class="sxs-lookup"><span data-stu-id="908f3-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="908f3-111">この作業は手動で行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="908f3-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="908f3-112">学習経路のマルチリンガルの概要を読む</span><span class="sxs-lookup"><span data-stu-id="908f3-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="908f3-113">マルチリンガルサポートが教育経路でどのように機能するかについては、「 [学習経路」](custom_overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="908f3-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview.md).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="908f3-114">更新の前提条件</span><span class="sxs-lookup"><span data-stu-id="908f3-114">Prerequisites to update</span></span>
<span data-ttu-id="908f3-115">学習経路を更新する前に、次の前提条件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="908f3-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="908f3-116">学習経路を更新するユーザーは、テナントのアプリカタログのサイトコレクションの所有者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="908f3-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="908f3-117">学習経路をプロビジョニングするユーザーがアプリカタログのサイトコレクションの所有者ではない場合は、 [次の手順を実行](addappadmin.md) して続行します。</span><span class="sxs-lookup"><span data-stu-id="908f3-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="908f3-118">言語設定を設定する</span><span class="sxs-lookup"><span data-stu-id="908f3-118">Set language settings</span></span> 
<span data-ttu-id="908f3-119">学習経路を更新する前に、サイトの言語設定を設定します。</span><span class="sxs-lookup"><span data-stu-id="908f3-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="908f3-120">ラーニングポイントサイトの多言語サポートを有効にするには、[ **ページとニュースを複数言語に翻訳** する] を **[オン**] に設定し、サイトに対してサポートする言語を追加します。</span><span class="sxs-lookup"><span data-stu-id="908f3-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="908f3-121">[ラーニングポイント] サイトで、右上から [ **設定** ] を選択し、[ **サイト情報**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="908f3-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="908f3-122">[サイト情報] ウィンドウの下部にある [ **すべてのサイト設定の表示**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="908f3-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="908f3-123">[ **サイトの管理**] で、[ **言語設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="908f3-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="908f3-124">[ **ページとニュースを複数の言語に翻訳できるよう**にする] で、切り替えスイッチを設定します。</span><span class="sxs-lookup"><span data-stu-id="908f3-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="908f3-125">Multiligual サイトの場合は、トグルを **[オン**] にして、[言語の追加] セクションに進みます。</span><span class="sxs-lookup"><span data-stu-id="908f3-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="908f3-126">英語のみのサイトの場合は、[ **オフ**] に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="908f3-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="908f3-127">言語を追加する</span><span class="sxs-lookup"><span data-stu-id="908f3-127">Add languages</span></span>
<span data-ttu-id="908f3-128">学習経路は9つの言語をサポートしているため、必要な言語のみを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="908f3-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="908f3-129">このドキュメントで使用されている例では、イタリア語が追加されています。</span><span class="sxs-lookup"><span data-stu-id="908f3-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="908f3-130">[ **サイト言語の追加または削除**] の下で、 **[言語の選択または入力**] で言語名の入力を開始するか、ドロップダウンから言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="908f3-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="908f3-131">複数の言語を追加するには、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="908f3-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="908f3-132">このページに戻ると、いつでもサイトで言語を追加または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="908f3-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="908f3-133">翻訳者を割り当てる</span><span class="sxs-lookup"><span data-stu-id="908f3-133">Assign translators</span></span>
<span data-ttu-id="908f3-134">学習経路の言語設定を定義するときは、翻訳者を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="908f3-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="908f3-135">翻訳者には外国語プロファイルを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="908f3-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="908f3-136">外国語プロファイルの詳細については、「 [多言語の通信サイト、ページ、ニュースを作成する](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="908f3-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="908f3-137">サポートされている言語の場合は、[ **トランスレーターの選択] また** は [翻訳者の入力] をクリックし、トランスレーターを選択します。</span><span class="sxs-lookup"><span data-stu-id="908f3-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="908f3-138">ラーニングパス web パーツパッケージを更新する</span><span class="sxs-lookup"><span data-stu-id="908f3-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="908f3-139">この手順では、ラーニング経路の 4.0 web パーツを SharePoint のアプリカタログにアップロードし、ラーニングポイント管理ページに移動して更新プロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="908f3-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="908f3-140">Web パーツパッケージをアップロードする</span><span class="sxs-lookup"><span data-stu-id="908f3-140">Upload the web part package</span></span>
1.  <span data-ttu-id="908f3-141">[GitHub カスタム学習リポジトリ](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)に移動し、[ **customlearning] sppkg**を選択して、それを PC のローカルドライブにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="908f3-141">Go to the [GitHub custom learning repository](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), select **customlearning.sppkg** and then download it to a local drive on your PC.</span></span>
2.  <span data-ttu-id="908f3-142">まだサインインしていない場合は、テナント管理者またはサイト コレクション管理者アカウントを使用して、テナントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="908f3-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="908f3-143">[**管理**] [  >  すべての SharePoint の機能**を表示] を**クリックし  >  **SharePoint**  >  **More Features**ます。</span><span class="sxs-lookup"><span data-stu-id="908f3-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="908f3-144">[ **アプリ**] の下にある [ **開く**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="908f3-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="908f3-145">[**アプリカタログ**  >  **の SharePoint 用アプリの配布**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="908f3-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="908f3-146">[**アップロード**  >  **ファイルの選択] を**クリックします。</span><span class="sxs-lookup"><span data-stu-id="908f3-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="908f3-147">ダウンロードした**customlearning**ファイルを選択し、[ **OK**Deploy] をクリックし  >  **Deploy**ます。</span><span class="sxs-lookup"><span data-stu-id="908f3-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="908f3-148">更新を完了する</span><span class="sxs-lookup"><span data-stu-id="908f3-148">Complete the update</span></span>
1.  <span data-ttu-id="908f3-149">[ラーニングの経路] サイトで、[**ホーム**] メニューから [**ラーニングパス管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="908f3-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="908f3-150">更新するかどうかを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="908f3-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="908f3-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="908f3-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="908f3-152">[**スタート**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="908f3-152">Click **Start**.</span></span> 
4. <span data-ttu-id="908f3-153">更新が完了したら、[ **閉じる**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="908f3-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="908f3-154">次の手順</span><span class="sxs-lookup"><span data-stu-id="908f3-154">Next Steps</span></span>
- <span data-ttu-id="908f3-155">サイトと web パーツで提供される [既定のコンテンツ](custom_exploresite.md) について説明します。</span><span class="sxs-lookup"><span data-stu-id="908f3-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="908f3-156">サイトページの翻訳の詳細については、「 [サイトページを翻訳](custom_translate_page_ml.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="908f3-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

