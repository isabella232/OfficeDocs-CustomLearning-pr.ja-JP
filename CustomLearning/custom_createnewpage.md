---
author: pkrebs
ms.author: pkrebs
title: プレイリストの SharePoint ページを作成する
ms.date: 02/10/2019
description: プレイリストの SharePoint ページを作成する
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055501"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="a134a-103">カスタムプレイリストの SharePoint ページを作成する</span><span class="sxs-lookup"><span data-stu-id="a134a-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="a134a-104">カスタム学習の固有の機能の1つとして、Microsoft や作成した SharePoint アセットから集められた再生リストを作成する機能があります。</span><span class="sxs-lookup"><span data-stu-id="a134a-104">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="a134a-105">この例では、再生リストを作成する前に SharePoint ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="a134a-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="a134a-106">SharePoint ページからプレイリストを作成する機能は、Microsoft または組織から入手可能な Web パーツを使用してページを作成するさまざまな機会を提供します。</span><span class="sxs-lookup"><span data-stu-id="a134a-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="a134a-107">たとえば、リストには、YouTube からのビデオが埋め込まれた SharePoint ページ、Office 365 フォームから作成されたフォーム、または組み込み Power BI レポートを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a134a-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="a134a-108">この例では、埋め込み web パーツとテキスト web パーツを使用してページを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a134a-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="a134a-109">カスタムプレイリストの SharePoint ページを作成する</span><span class="sxs-lookup"><span data-stu-id="a134a-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="a134a-110">SharePoint**歯車**アイコンをクリックし、[**ページの追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a134a-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="a134a-111">ページの左側にある [**新しいセクションの追加] (+)** をクリックし、[セクションレイアウト] で [ **2 列**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a134a-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="a134a-112">左側の列で、[+] をクリックし、[**埋め込み**web パーツ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a134a-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="a134a-113">右の列で、[+] をクリックし、[**テキスト**web パーツ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a134a-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="a134a-114">ページは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="a134a-114">Your page should look like this.</span></span>

![cg-pagenewstart](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="a134a-116">YouTube からのビデオおよびテキストの追加</span><span class="sxs-lookup"><span data-stu-id="a134a-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="a134a-117">ブラウザーで、[YouTube] に移動します。</span><span class="sxs-lookup"><span data-stu-id="a134a-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="a134a-118">この例では、「Office 365 – Microsoft のベストプロダクティビティアプリ」を検索します。</span><span class="sxs-lookup"><span data-stu-id="a134a-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="a134a-119">ビデオをクリックして再生し、一時停止して、それを右クリックします。</span><span class="sxs-lookup"><span data-stu-id="a134a-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="a134a-120">[**埋め込みコードのコピー**] をクリックし、SharePoint ページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="a134a-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="a134a-121">**埋め込み**web パーツで [**埋め込みコードの追加**] をクリックし、YouTube ビデオからコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="a134a-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="a134a-122">[YouTube] ページに戻り、ビデオの**説明**テキストをコピーします。</span><span class="sxs-lookup"><span data-stu-id="a134a-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="a134a-123">SharePoint ページに戻り、**テキスト**web パーツを選択してから、YouTube ビデオからテキストをコピーします。</span><span class="sxs-lookup"><span data-stu-id="a134a-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="a134a-124">SharePoint ページのタイトル領域で [ **web パーツの編集**] アイコンを選択し、そのページに「Custom プレイリストの紹介」という名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="a134a-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="a134a-125">[**レイアウト**] で、[**プレーン**] を選択し、[**タイトル領域**のプロパティ] ウィンドウを閉じます。</span><span class="sxs-lookup"><span data-stu-id="a134a-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="a134a-126">これで、ページは次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="a134a-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="a134a-128">ページの発行</span><span class="sxs-lookup"><span data-stu-id="a134a-128">Publish the page</span></span>

- <span data-ttu-id="a134a-129">[**発行**] ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="a134a-129">Select the **Publish** button.</span></span> <span data-ttu-id="a134a-130">これで、この SharePoint ページをカスタムプレイリストに追加する準備ができました。</span><span class="sxs-lookup"><span data-stu-id="a134a-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 