---
author: karuanag
ms.author: karuanag
title: プレイリストをカスタマイズして共有する
ms.date: 02/10/2019
description: 既存のコンテンツまたは新しい SharePoint ページからカスタム再生リストを作成する
ms.service: sharepoint online
ms.openlocfilehash: 6258668b417ba496c7ac75e36ce2bc1f1dae27a5
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233809"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="c69e0-103">プレイリストをカスタマイズして共有する</span><span class="sxs-lookup"><span data-stu-id="c69e0-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="c69e0-104">再生リストを作成する</span><span class="sxs-lookup"><span data-stu-id="c69e0-104">Create a Playlist</span></span>

<span data-ttu-id="c69e0-105">再生リストは、"assets" の compliation です。</span><span class="sxs-lookup"><span data-stu-id="c69e0-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="c69e0-106">"アセット" は、SharePoint ページまたは Microsoft トレーニングコンテンツの既存のアイテムです。</span><span class="sxs-lookup"><span data-stu-id="c69e0-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="c69e0-107">再生リストを作成するときに、ユーザーに対して学習パスを作成するために一緒に使用するアセットを選択します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="c69e0-108">SharePoint ページを追加する利点は、自分の組織でホストされている YouTube ビデオまたはビデオを使用して SharePoint ページを作成できることです。</span><span class="sxs-lookup"><span data-stu-id="c69e0-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="c69e0-109">フォームまたはその他の Office 365 コンテンツを含むページを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="c69e0-110">手順 1: プレイリストの SharePoint ページを作成する</span><span class="sxs-lookup"><span data-stu-id="c69e0-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="c69e0-111">この例では、まず、プレイリストに追加する SharePoint ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="c69e0-112">YouTube のビデオ web パーツとテキスト web パーツを使用してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="c69e0-113">これらの手順では、SharePoint Online サービスを使用していることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="c69e0-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="c69e0-114">新しいページを作成する</span><span class="sxs-lookup"><span data-stu-id="c69e0-114">Create a new page</span></span>
1.  <span data-ttu-id="c69e0-115">[設定] メニューを選択し > サイトコンテンツ > サイトページ > 新しい > サイトページにします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="c69e0-116">タイトル領域で、「Teams コマンドボックスを使用する」と入力します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="c69e0-117">[新しい項目の追加] を選択し、[2 列] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-117">Select the Add a new section, and then select Two Columns.</span></span>

![2列の追加](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="c69e0-119">左側のボックスで、[新しい web パーツの追加] を選択し、[埋め込み] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="c69e0-120">Web ブラウザーでこの URL に移動し、 https://youtu.be/wYrRCRphrp0 ビデオの埋め込みコードを取得します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="c69e0-121">SharePoint Web パーツで、[埋め込みコードの追加] を選択し、[埋め込み] ボックスに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="c69e0-122">右側のボックスで、[新しい web パーツの追加] を選択し、[テキスト] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="c69e0-123">Web ブラウザーで、次の URL に移動 https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b して、Try! をコピーします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="c69e0-124">ページの指示に従って、テキスト Web パーツに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="c69e0-125">ページは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="c69e0-125">Your page should look like the following.</span></span> 

![埋め込みページ](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="c69e0-127">[ **発行**] をクリックし、ページの URL をコピーしてメモ帳に貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="c69e0-128">手順 2: 再生リストを作成する</span><span class="sxs-lookup"><span data-stu-id="c69e0-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="c69e0-129">サイトの操作でカスタムの [ **ラーニング管理** ] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="c69e0-130">![custom_admin.png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="c69e0-130">![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="c69e0-131">**カテゴリ**が選択されていることを確認する</span><span class="sxs-lookup"><span data-stu-id="c69e0-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="c69e0-132">新しいプレイリストが表示されるようにするカテゴリをクリックします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="c69e0-133">カテゴリ名の横にあるプラス記号 (+) をクリックし ![custom_addplay.png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="c69e0-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="c69e0-134">次の例のように値を入力し、[ **作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="c69e0-135">![custom_details.png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="c69e0-135">![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="c69e0-136">**タイトル** -再生リストの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="c69e0-137">**説明** -学習される内容に関する情報</span><span class="sxs-lookup"><span data-stu-id="c69e0-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="c69e0-138">**カテゴリ** -最初の選択範囲に基づいて事前設定</span><span class="sxs-lookup"><span data-stu-id="c69e0-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="c69e0-139">**サブカテゴリ** -初期の選択に基づいて事前設定</span><span class="sxs-lookup"><span data-stu-id="c69e0-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="c69e0-140">**テクノロジ** -該当する場合に選択します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="c69e0-141">**レベル** -初級、intermidate または Advanced</span><span class="sxs-lookup"><span data-stu-id="c69e0-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="c69e0-142">**対象ユーザー** -これにより、Microsoft によって提供される定義済みのロールのリストに基づいてコンテンツを対象とすることができます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="c69e0-143">[**詳細の保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="c69e0-144">再生リストのアイコンイメージをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="c69e0-145">イメージアイコンをクリックして、以前にアップロードしたイメージの URL を挿入します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="c69e0-146">画像が、カスタム学習サイトコレクション内にあるか、またはすべてのユーザーがファイルにアクセスできる別の場所に配置されているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="c69e0-147">![custom_image.png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="c69e0-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="c69e0-148">手順 3: 再生リストにアセットを追加する</span><span class="sxs-lookup"><span data-stu-id="c69e0-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="c69e0-149">この手順では、Microsoft の既存のアセットと、プレイリストに作成した SharePoint ページを追加します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="c69e0-150">再生リストの詳細を保存すると、既存のアセットの検索を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="c69e0-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="c69e0-151">**任意の検索用語を入力** して、他の再生リストから利用できる定義済みのアセットの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="c69e0-152">アセットの**名前をクリックし**て、新しい再生リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-152">**Click on the name** of an asset to include it in your new playlist.</span></span>
<span data-ttu-id="c69e0-153">![custom_slist.png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="c69e0-153">![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="c69e0-154">また、前の手順で作成した SharePoint ページを追加したり、表示で最初から作成したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="c69e0-155">[再生リストアセット] ダイアログボックスの [ **新しいアセット** ] オプションをクリックします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="c69e0-156">アセットに **タイトル**を付けます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-156">Give your asset a **Title**.</span></span> <span data-ttu-id="c69e0-157">入力すると、追加のオプションcustom_newpage.png表示されます。 ![](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="c69e0-157">Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="c69e0-158">これで、SharePoint Online に新しいアセットページを作成したり、既存のページの URL を入力してカスタムプレイリストに追加したりできます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="c69e0-159">**Category**、 **Sub Category** 、および **ts** の各フィールドは、このプレイリストの以前の選択に基づいて事前に入力されます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="c69e0-160">この各資産のレベルと対象ユーザーを適切に選択してください。</span><span class="sxs-lookup"><span data-stu-id="c69e0-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="c69e0-161">[ **アセットの保存** ] をクリックして、カスタムプレイリストに追加します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="c69e0-162">再生リストが完成するまで、個々のページを検索または追加するには、これらの手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c69e0-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="c69e0-163">[ **再生リストを閉じる** ] をクリックして保存する</span><span class="sxs-lookup"><span data-stu-id="c69e0-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="c69e0-164">これで、このコンテンツを含むプレイリストは、カスタム学習 web パーツをインストールまたは埋め込まれた任意の場所で利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="c69e0-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="c69e0-165">再生リストを閉じた後で間違いを犯した場合は、再生リスト名の横にある X をクリックしてそのカテゴリから削除できます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="c69e0-166">検討事項</span><span class="sxs-lookup"><span data-stu-id="c69e0-166">Things to Think About</span></span>

<span data-ttu-id="c69e0-167">カスタム再生リストを使用すると、エンドユーザーにさまざまなタスクをサポートできます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-167">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="c69e0-168">休暇を申請するフォームがあるかどうか</span><span class="sxs-lookup"><span data-stu-id="c69e0-168">Do you have a time off request form?</span></span>  <span data-ttu-id="c69e0-169">ハードウェア機器を要求するフォーム</span><span class="sxs-lookup"><span data-stu-id="c69e0-169">A form to request hardware equipment?</span></span>  <span data-ttu-id="c69e0-170">既存のトレーニング資産はすべて、そのままの方法で作業できます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-170">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="c69e0-171">共有のプレイリスト</span><span class="sxs-lookup"><span data-stu-id="c69e0-171">Share Playlists</span></span>

1. <span data-ttu-id="c69e0-172">Webpart 内の任意のプレイリストまたはサイトの操作に移動する</span><span class="sxs-lookup"><span data-stu-id="c69e0-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="c69e0-173">左上隅に3つのアイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="c69e0-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="c69e0-174">リンクを表すアイコンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="c69e0-175">URL を再生リストにコピーします。</span><span class="sxs-lookup"><span data-stu-id="c69e0-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="c69e0-176">![share.png](media/share.png) この URL をサイトナビゲーションに挿入したり、他の通信で使用したりして、従業員をその再生リストに直接移動することができるようになります。</span><span class="sxs-lookup"><span data-stu-id="c69e0-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="c69e0-177">次の手順- [ドライブの採用](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="c69e0-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
