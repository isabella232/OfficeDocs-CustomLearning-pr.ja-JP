---
author: pkrebs
ms.author: pkrebs
title: カスタム学習アセットへのリンク
ms.date: 02/15/2019
description: カスタム学習アセットにリンクする方法
ms.openlocfilehash: cdde37f370663ca50241833a15e8411921b45a1b
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056161"
---
# <a name="link-to-custom-learning-content"></a><span data-ttu-id="ed84b-103">カスタム学習コンテンツへのリンク</span><span class="sxs-lookup"><span data-stu-id="ed84b-103">Link to Custom Learning content</span></span>

<span data-ttu-id="ed84b-104">カスタム学習を使用すると、次の2つの方法でコンテンツにリンクすることができます。</span><span class="sxs-lookup"><span data-stu-id="ed84b-104">With Custom Learning, there are two ways to link to content:</span></span>

- <span data-ttu-id="ed84b-105">表示するコンテンツに対してフィルター処理された Web パーツをホストするページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-105">Link to the page that host the Web part filtered for the content you want to display.</span></span> 
- <span data-ttu-id="ed84b-106">Web パーツのインスタンスへの直接リンク</span><span class="sxs-lookup"><span data-stu-id="ed84b-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="ed84b-107">ページへのリンク</span><span class="sxs-lookup"><span data-stu-id="ed84b-107">Link to a page</span></span>

<span data-ttu-id="ed84b-108">カスタム学習 Web パーツで新しいページと学習経験を作成した場合は、表示するコンテンツを表示するように構成された Web パーツを使用してページにリンクできます。</span><span class="sxs-lookup"><span data-stu-id="ed84b-108">If you've created new pages and learning experiences with the Custom Learning Web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="ed84b-109">前のセクションでは、Excel の再生リストをページに表示する方法について説明しました。</span><span class="sxs-lookup"><span data-stu-id="ed84b-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="ed84b-110">これで、ホームページを編集してページにリンクすることができました。</span><span class="sxs-lookup"><span data-stu-id="ed84b-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="ed84b-111">ホームページで、[**編集**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="ed84b-112">ホームページのタイルのいずれかで [**詳細の編集**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="ed84b-113">この例では、推奨さ**れるプレイリスト**のタイルを編集します。</span><span class="sxs-lookup"><span data-stu-id="ed84b-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="ed84b-114">[**リンク**] で、[**変更**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-114">Under **Link**, click **Change**.</span></span>

![cg-linktopage](media/cg-linktopage.png)

4. <span data-ttu-id="ed84b-116">[**サイト**]、[**サイトページ**] の順にクリックしてリンク先のページをクリックし、[**開く**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="ed84b-117">この例では、前のセクションで説明した**Create-your-own-experience**ページにリンクします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="ed84b-118">[ヒーローのプロパティ] ウィンドウを閉じ、[**発行**] をクリックして、リンクをテストします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-custom-learning-web-part"></a><span data-ttu-id="ed84b-119">カスタム学習 web パーツへのリンク</span><span class="sxs-lookup"><span data-stu-id="ed84b-119">Link to the Custom Learning web part</span></span>
<span data-ttu-id="ed84b-120">カスタム学習を使用すると、管理者またはエンドユーザーは、web パーツを含むページに依存しない web パーツのインスタンスにリンクすることができます。</span><span class="sxs-lookup"><span data-stu-id="ed84b-120">Custom Learning gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="ed84b-121">コピーしたリンクやリンクを他のページから共有することができます。</span><span class="sxs-lookup"><span data-stu-id="ed84b-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="ed84b-122">コピーされたリンクをクリックすると、CustomLLearningViewer ページにカスタム学習 web パーツインスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ed84b-122">The copied link, when clicked, shows the Custom Learning web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="ed84b-123">1 つの例を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="ed84b-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="ed84b-124">ホームページで、[ **Office 365 トレーニング**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-124">From the Home page, click **Office 365 training**.</span></span>
2. <span data-ttu-id="ed84b-125">[ **microsoft teams**] をクリックし、[ **microsoft teams への導入] を**クリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="ed84b-126">[**コピー** ] アイコンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-126">Click the **Copy** icon.</span></span>

![cg-linktowebpart](media/cg-linktowebpart.png)

4. <span data-ttu-id="ed84b-128">カスタム学習メニューから [ホーム] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ed84b-128">Click Home from the Custom Learning menu.</span></span>
5. <span data-ttu-id="ed84b-129">コピーした URL をブラウザーのアドレスバーに貼り付けて、enter キーを押します。</span><span class="sxs-lookup"><span data-stu-id="ed84b-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="ed84b-130">次の図に示すように、リンクは CustomLearningViewer ページにジャンプし、コピーされたリンクのパラメーターに基づいてコンテンツを表示します。</span><span class="sxs-lookup"><span data-stu-id="ed84b-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![cg-linktowebpartviewer](media/cg-linktowebpartviewer.png)

