---
author: karuanag
ms.author: karuanag
manager: alexb
title: プレイリストのカスタマイズと共有
ms.date: 02/10/2019
description: 既存のコンテンツまたは新しい SharePoint ページからカスタム プレイリストを作成する
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000213"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="b32fc-103">プレイリストのカスタマイズと共有</span><span class="sxs-lookup"><span data-stu-id="b32fc-103">Customize and share playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="b32fc-104">プレイリストの作成</span><span class="sxs-lookup"><span data-stu-id="b32fc-104">Create a Playlist</span></span>

<span data-ttu-id="b32fc-105">プレイリストは"アセット" の賛辞です。</span><span class="sxs-lookup"><span data-stu-id="b32fc-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="b32fc-106">"アセット" は、SharePoint ページまたは Microsoft トレーニング コンテンツの既存のアイテムです。</span><span class="sxs-lookup"><span data-stu-id="b32fc-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="b32fc-107">プレイリストを作成するときに、一緒に移動するアセットを選択して、ユーザーの学習パスを作成します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="b32fc-108">SharePoint ページを追加する利点は、組織内でホストされている YouTube ビデオまたはビデオを使用して SharePoint ページを作成できる点です。</span><span class="sxs-lookup"><span data-stu-id="b32fc-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="b32fc-109">Forms または他の 365 コンテンツを使用してOffice作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="b32fc-110">手順 1: プレイリストの SharePoint ページを作成する</span><span class="sxs-lookup"><span data-stu-id="b32fc-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="b32fc-111">この例では、まずプレイリストに追加する SharePoint ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="b32fc-112">YouTube ビデオ Web パーツとテキスト Web パーツを含むページを作成します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="b32fc-113">これらの手順では、SharePoint Online サービスを使用している必要があります。</span><span class="sxs-lookup"><span data-stu-id="b32fc-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="b32fc-114">新しいページを作成する</span><span class="sxs-lookup"><span data-stu-id="b32fc-114">Create a new page</span></span>
1.  <span data-ttu-id="b32fc-115">[サイト ページ] の [>] >[サイト ページ>] >を選択します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="b32fc-116">タイトル領域で、「Teams コマンド ボックスを使用する」と入力します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="b32fc-117">[新しい追加] セクションを選択し、[2 つの列] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-117">Select the Add a new section, and then select Two Columns.</span></span>

![2 列の追加](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="b32fc-119">左側のボックスで、[新しい Web パーツの追加] を選択し、[埋め込み] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="b32fc-120">Web ブラウザーで、この URL に移動 https://youtu.be/wYrRCRphrp0 し、ビデオの埋め込みコードを取得します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="b32fc-121">SharePoint Web パーツで、[埋め込みコードの追加] を選択し、[埋め込み] ボックスに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="b32fc-122">右側のボックスで、[新しい Web パーツの追加] を選択し、[テキスト] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="b32fc-123">Web ブラウザーで、次の URL に移動し https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 、[試す] をコピーします。</span><span class="sxs-lookup"><span data-stu-id="b32fc-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="b32fc-124">ページの手順とテキスト Web パーツに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="b32fc-125">ページは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="b32fc-125">Your page should look like the following.</span></span> 
<span data-ttu-id="b32fc-126">![[埋め込み] ページ](media/clo365teamscommandbox.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-126">![Embed page](media/clo365teamscommandbox.png)</span></span>
9.  <span data-ttu-id="b32fc-127">[ **発行]** をクリックし、ページの URL をコピーしてメモ帳に貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="b32fc-128">手順 2: プレイリストを作成する</span><span class="sxs-lookup"><span data-stu-id="b32fc-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="b32fc-129">サイト エクスペリエンスの **[カスタム学習管理** ] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="b32fc-130">![[カスタム学習管理] を選択する画面。](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-130">![Screen where you select Custom Learning Administration.](media/custom_admin.png)</span></span>
1. <span data-ttu-id="b32fc-131">[カテゴリ **] が選択** されているのを確認する</span><span class="sxs-lookup"><span data-stu-id="b32fc-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="b32fc-132">新しいプレイリストを表示するカテゴリをクリックします</span><span class="sxs-lookup"><span data-stu-id="b32fc-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="b32fc-133">カテゴリ名の横にあるプラス記号ウィンドウをクリックし、[カテゴリ] オプションを選択し、 ![ プラス記号を強調表示します。](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-133">Next to the category name, click on the plus symbol ![Window with the Category option and the Plus sign highlighted.](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="b32fc-134">下の例に示すように値を入力し、[作成] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="b32fc-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="b32fc-135">![プレイリストの詳細を入力するページ。](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-135">![Page where you enter playlist details.](media/custom_details.png)</span></span>
- <span data-ttu-id="b32fc-136">**タイトル** - プレイリストの表示名</span><span class="sxs-lookup"><span data-stu-id="b32fc-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="b32fc-137">**説明** - 学習内容に関する情報</span><span class="sxs-lookup"><span data-stu-id="b32fc-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="b32fc-138">**カテゴリ** - 最初の選択に基づいて事前に選択されます</span><span class="sxs-lookup"><span data-stu-id="b32fc-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="b32fc-139">**Sub Category** - intial 選択範囲に基づいて事前に選択されている</span><span class="sxs-lookup"><span data-stu-id="b32fc-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="b32fc-140">**テクノロジ** - 該当する場合に選択する</span><span class="sxs-lookup"><span data-stu-id="b32fc-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="b32fc-141">**レベル** - ビギナー、インターミダテ、または Advanced</span><span class="sxs-lookup"><span data-stu-id="b32fc-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="b32fc-142">**対象** ユーザー - Microsoft が提供する定義済みの役割の一覧に基づいてコンテンツをターゲットに設定できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="b32fc-143">[詳細 **の保存] をクリックします。**</span><span class="sxs-lookup"><span data-stu-id="b32fc-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="b32fc-144">プレイリストのアイコンイメージをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="b32fc-145">画像アイコンをクリックし、以前にアップロードした画像の URL を挿入します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="b32fc-146">イメージがカスタム ラーニング サイト コレクション内にあるか、すべてのユーザーがファイルにアクセスできる別の場所に保存されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b32fc-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="b32fc-147">![イメージ ウィンドウを選択します。](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-147">![Choose an image window.](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="b32fc-148">手順 3: プレイリストにアセットを追加する</span><span class="sxs-lookup"><span data-stu-id="b32fc-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="b32fc-149">この手順では、Microsoft の既存のアセットと、作成した SharePoint ページをプレイリストに追加します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="b32fc-150">プレイリストの詳細を保存したら、既存のアセットの検索を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="b32fc-151">**任意の検索用語を入力** して、他のプレイリストから使用できる定義済みのアセットの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="b32fc-152">**アセットの名前をクリック** して、新しいプレイリストに含める。</span><span class="sxs-lookup"><span data-stu-id="b32fc-152">**Click on the name** of an asset to include it in your new playlist.</span></span><br/>
<span data-ttu-id="b32fc-153">![プレイリストのアセット ページ](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-153">![Playlist assets page](media/custom_slist.png)</span></span>

<span data-ttu-id="b32fc-154">以前に作成した SharePoint ページを追加したり、エクスペリエンスで最初から作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="b32fc-155">[プレイリストアセット] **ダイアログの** [新しいアセット] オプションをクリックします。</span><span class="sxs-lookup"><span data-stu-id="b32fc-155">Click on the **New Asset** option in the Playlist Assets dialog.</span></span>
1. <span data-ttu-id="b32fc-156">アセットに Title を **指定します**。</span><span class="sxs-lookup"><span data-stu-id="b32fc-156">Give your asset a **Title**.</span></span> <span data-ttu-id="b32fc-157">入力すると、追加のオプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-157">Once entered, additional options will display.</span></span>
<span data-ttu-id="b32fc-158">![タイトルと追加の詳細を入力するフォーム。](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-158">![Form where you enter your title and additional details.](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="b32fc-159">SharePoint Online で新しいアセット ページを作成するか、既存のページの URL を入力してカスタム プレイリストに追加できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-159">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="b32fc-160">**[カテゴリ\*\*\*\*] 、[サブ カテゴリ\*\*\*\*]** フィールド、および [テクノロジ] フィールドは、このプレイリストの以前の選択内容に基づいて事前に入力されます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-160">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="b32fc-161">この個々のアセットのレベルと対象ユーザーに対して適切な選択を行います。</span><span class="sxs-lookup"><span data-stu-id="b32fc-161">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="b32fc-162">[ **アセットの保存]** をクリックしてカスタム プレイリストに追加する</span><span class="sxs-lookup"><span data-stu-id="b32fc-162">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="b32fc-163">プレイリストが完了するまで、個々のページを検索または追加する手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="b32fc-163">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="b32fc-164">[プレイリスト **を閉じる] を** クリックして保存する</span><span class="sxs-lookup"><span data-stu-id="b32fc-164">Click **Close Playlist** to save</span></span>

<span data-ttu-id="b32fc-165">このコンテンツを含むプレイリストは、Custom Learning webpart をインストール/埋め込み済みの場所で利用できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-165">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="b32fc-166">プレイリストを閉じた後に間違いを犯した場合は、プレイリスト名の横にある [X] をクリックして、カテゴリから削除できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-166">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="b32fc-167">考え方</span><span class="sxs-lookup"><span data-stu-id="b32fc-167">Things to Think About</span></span>

<span data-ttu-id="b32fc-168">カスタムプレイリストは、さまざまなタスクでエンド ユーザーを支援するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-168">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="b32fc-169">時間外の要求フォームはありますか?</span><span class="sxs-lookup"><span data-stu-id="b32fc-169">Do you have a time off request form?</span></span>  <span data-ttu-id="b32fc-170">ハードウェア機器を要求するフォーム</span><span class="sxs-lookup"><span data-stu-id="b32fc-170">A form to request hardware equipment?</span></span>  <span data-ttu-id="b32fc-171">既存のトレーニングアセットは、エクスペリエンスにプログラムできます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-171">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="b32fc-172">プレイリストを共有する</span><span class="sxs-lookup"><span data-stu-id="b32fc-172">Share Playlists</span></span>

1. <span data-ttu-id="b32fc-173">Web パーツまたはサイト エクスペリエンス内の任意のプレイリストに移動する</span><span class="sxs-lookup"><span data-stu-id="b32fc-173">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="b32fc-174">左上隅に 3 つのアイコンが表示されます</span><span class="sxs-lookup"><span data-stu-id="b32fc-174">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="b32fc-175">リンクを表すアイコンをクリックする</span><span class="sxs-lookup"><span data-stu-id="b32fc-175">Click on the icon representing a link</span></span>
1. <span data-ttu-id="b32fc-176">URL をプレイリストにコピー ![ する 画面 URL の横にある [コピー] をクリックします。](media/share.png)</span><span class="sxs-lookup"><span data-stu-id="b32fc-176">Copy the URL to the playlist ![Screen where you click Copy next to the URL.](media/share.png)</span></span>
<span data-ttu-id="b32fc-177">この URL は、サイト ナビゲーションに挿入したり、他のコミュニケーションで利用したりして、従業員をそのプレイリストに直接移動できます。</span><span class="sxs-lookup"><span data-stu-id="b32fc-177">This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="b32fc-178">次の手順 - [導入の促進](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="b32fc-178">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
