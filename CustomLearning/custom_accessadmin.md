---
author: pkrebs
ms.author: pkrebs
title: カスタム学習管理ページにアクセスする
ms.date: 02/15/2019
description: Web パーツまたはメニューからカスタム学習管理ページにアクセスする方法
ms.openlocfilehash: e08d8dfc6690d9c5d26cd03efd780bbd27d72cd6
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/21/2019
ms.locfileid: "34327228"
---
# <a name="access-the-custom-learning-administration-page"></a><span data-ttu-id="0328b-103">カスタム学習管理ページにアクセスする</span><span class="sxs-lookup"><span data-stu-id="0328b-103">Access the Custom Learning Administration page</span></span>

<span data-ttu-id="0328b-104">カスタム学習管理ページは、Microsoft 365 Learning pathの web パーツを管理するための中心的な制御ポイントです。</span><span class="sxs-lookup"><span data-stu-id="0328b-104">The Custom Learning Administration page is the central controlling point for administration of the Microsoft 365 learning pathwasy web part.</span></span> <span data-ttu-id="0328b-105">ラーニングパス管理ページは、SharePoint 管理者のみが使用できます。</span><span class="sxs-lookup"><span data-stu-id="0328b-105">The learning pathways Administration page is only available to SharePoint Administrators.</span></span> <span data-ttu-id="0328b-106">サイトを訪問するメンバー権限を持つユーザーには、[**プレイリストの管理**] オプションは表示されません。</span><span class="sxs-lookup"><span data-stu-id="0328b-106">Users with member privileges visiting the site will not see the **Administer Playlist** option.</span></span> <span data-ttu-id="0328b-107">さらに、管理者のみが SharePoint**ホーム**メニューアイテムからカスタム学習管理ページを開くことができます。</span><span class="sxs-lookup"><span data-stu-id="0328b-107">In addition, only Administrators will have the ability to open the Custom Learning Administration page from the SharePoint **Home** menu item.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="0328b-108">製品のサブカテゴリまたは再生リストを非表示にするなど、カスタム学習管理ページで行われた変更は、Web パーツのすべてのインスタンスに反映されます。</span><span class="sxs-lookup"><span data-stu-id="0328b-108">Changes made on the Custom Learning Administration page, such as hiding a product subcategory or playlist, will be reflected in all instances of the Web part.</span></span> <span data-ttu-id="0328b-109">さらに、複数のユーザーが同時にカスタム学習管理を使用している場合には、カスタム学習では競合検出が提供されないため、管理者は1人だけがカスタム学習管理ページで変更を行うことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0328b-109">In addition, it’s recommended that only one administrator at time make changes on the Custom Learning Administrator page, since Custom Learning does not provide collision detection if multiple people are using the Custom Learning Administration at the same time.</span></span>  

## <a name="access-from-the-custom-learning-web-part---preferred-method"></a><span data-ttu-id="0328b-110">カスタム学習 Web パーツからのアクセス-推奨される方法</span><span class="sxs-lookup"><span data-stu-id="0328b-110">Access from the Custom Learning Web part - preferred method</span></span>
<span data-ttu-id="0328b-111">この例では、新しいブラウザーウィンドウで管理ページを開いているため、web パーツからカスタム学習管理ページを開くことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0328b-111">As we'll show you in this example, opening the Custom Learning Administration page from the web part is the preferred method since it opens the Admin page in a new browser window.</span></span> <span data-ttu-id="0328b-112">このメソッドを使用すると、タブ付きページ間を前後にめくって作業をチェックしたり、変更したりするのは簡単です。</span><span class="sxs-lookup"><span data-stu-id="0328b-112">With this method, it's easy to flip back and forth between the tabbed pages to check or modify your work.</span></span>  

1. <span data-ttu-id="0328b-113">Microsoft 365 learning の経路のホームページから、 **Office 365 のトレーニング**タイルをクリックします。</span><span class="sxs-lookup"><span data-stu-id="0328b-113">From the Microsoft 365 learning pathways Home page, click the **Office 365 training** tile.</span></span>
2. <span data-ttu-id="0328b-114">[**システム**] メニューの [**プレイリストの管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0328b-114">Click the **System** menu, then click **Administer Playlist**.</span></span> 

![cg-adminaccbtn](media/cg-adminaccbtn.png)

## <a name="access-from-the-home-menu-item"></a><span data-ttu-id="0328b-116">ホームメニュー項目からのアクセス</span><span class="sxs-lookup"><span data-stu-id="0328b-116">Access from the Home menu item</span></span>
<span data-ttu-id="0328b-117">管理者は、Web パーツを含むページに移動するのではなく、SharePoint**ホーム**メニューの項目から Microsoft learning 管理ページにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0328b-117">Rather than navigate to a page with a Web part, administrators can access the Microsoft learning adminstration page from the SharePoint **Home** menu item.</span></span> 

- <span data-ttu-id="0328b-118">Microsoft 365 Learning の経路のホームページで、[**ホーム**] メニューをクリックし、[ **Microsoft Learning administration**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0328b-118">From the Microsoft 365 Learning Pathways Home page, click the **Home** menu, then click **Microsoft learning administration**.</span></span>

![cg-adminaccmenu](media/cg-adminaccmenu.png)