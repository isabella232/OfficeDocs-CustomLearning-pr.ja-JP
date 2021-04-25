---
author: pkrebs
ms.author: pkrebs
title: プレイリストの SharePoint ページを作成する
ms.date: 02/10/2019
description: プレイリストの SharePoint ページを作成する
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999093"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="a50f2-103">カスタム プレイリスト用の SharePoint ページの作成</span><span class="sxs-lookup"><span data-stu-id="a50f2-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="a50f2-104">学習経路のユニークな機能の 1 つは、Microsoft のアセットと作成した SharePoint アセットから組み立てられたプレイリストを作成する機能です。</span><span class="sxs-lookup"><span data-stu-id="a50f2-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="a50f2-105">この例では、プレイリストを作成する前に SharePoint ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="a50f2-106">SharePoint ページからプレイリストを作成する機能は、Microsoft または組織から利用可能な Web パーツを使用してページを作成するさまざまな機会を提供します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="a50f2-107">たとえば、プレイリストには、YouTube の埋め込みビデオを含む SharePoint ページや、Office 365 フォームから作成されたフォーム、または埋め込み Power BI レポートを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a50f2-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="a50f2-108">この例では、埋め込み Web パーツとテキスト Web パーツを使用してページを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="a50f2-109">カスタム プレイリストの SharePoint ページを作成する</span><span class="sxs-lookup"><span data-stu-id="a50f2-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="a50f2-110">[SharePoint **Gear] アイコンを** クリックし、[ページの追加 **] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="a50f2-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="a50f2-111">ページ **の左側にある [新しいセクションの追加] (+)** をクリックし、セクション レイアウトの [2 つの **列** ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a50f2-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="a50f2-112">左側の列で、[+] をクリックし、[埋め込み] **Web パーツを** クリックします。</span><span class="sxs-lookup"><span data-stu-id="a50f2-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="a50f2-113">右側の列で、[+] をクリックし、[ **テキスト] Web パーツを** クリックします。</span><span class="sxs-lookup"><span data-stu-id="a50f2-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="a50f2-114">ページは次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="a50f2-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="a50f2-116">YouTube からビデオとテキストを追加する</span><span class="sxs-lookup"><span data-stu-id="a50f2-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="a50f2-117">ブラウザーで、YouTube に移動します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="a50f2-118">この例では、"365 Office Microsoft の最高の生産性アプリ" を検索します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="a50f2-119">ビデオをクリックして再生し、一時停止してから右クリックします。</span><span class="sxs-lookup"><span data-stu-id="a50f2-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="a50f2-120">[埋 **め込みコードのコピー]** をクリックし、SharePoint ページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="a50f2-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="a50f2-121">[ **埋め込み] Web** パーツで **[埋** め込みコードの追加] をクリックし、YouTube ビデオからコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="a50f2-122">YouTube ページに戻り、ビデオの **説明テキスト** をコピーします。</span><span class="sxs-lookup"><span data-stu-id="a50f2-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="a50f2-123">SharePoint ページに戻り、 **テキスト Web** パーツを選択し、YouTube ビデオからテキストをコピーします。</span><span class="sxs-lookup"><span data-stu-id="a50f2-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="a50f2-124">[SharePoint] **ページの [** タイトル] 領域で [Web パーツの編集] アイコンを選択し、[カスタム プレイリストの概要] ページに名前を付きます。</span><span class="sxs-lookup"><span data-stu-id="a50f2-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="a50f2-125">[ **レイアウト] で**、[プレーン] **を** 選択し、[タイトル領域] プロパティ **ウィンドウ** を閉じます。</span><span class="sxs-lookup"><span data-stu-id="a50f2-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="a50f2-126">これで、ページは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="a50f2-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="a50f2-128">ページを発行する</span><span class="sxs-lookup"><span data-stu-id="a50f2-128">Publish the page</span></span>

- <span data-ttu-id="a50f2-129">[発行] **ボタンを選択** します。</span><span class="sxs-lookup"><span data-stu-id="a50f2-129">Select the **Publish** button.</span></span> <span data-ttu-id="a50f2-130">これで、この SharePoint ページをカスタム プレイリストに追加する準備ができました。</span><span class="sxs-lookup"><span data-stu-id="a50f2-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 