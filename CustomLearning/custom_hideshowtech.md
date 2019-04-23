---
author: pkrebs
ms.author: pkrebs
title: テクノロジの非表示と表示
ms.date: 02/15/2019
description: テクノロジを非表示にして表示する方法
ms.openlocfilehash: 38b814b85d4e060e5387b2173476c455cfcf7160
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055671"
---
# <a name="hide-and-show-technology"></a><span data-ttu-id="807a8-103">テクノロジの非表示と表示</span><span class="sxs-lookup"><span data-stu-id="807a8-103">Hide and show Technology</span></span>

<span data-ttu-id="807a8-104">場合によっては、組織でサポートされていないテクノロジのコンテンツを非表示にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="807a8-104">In some cases, you’ll want to hide content for a technology that’s not supported in your organization.</span></span> <span data-ttu-id="807a8-105">[テクノロジの非表示機能は、Web パーツ全体にわたってテクノロジが表示されないようにすることを目的としています。</span><span class="sxs-lookup"><span data-stu-id="807a8-105">The Hide Technology feature is designed to prevent technology from appearing throughout the Web part.</span></span> <span data-ttu-id="807a8-106">これにより、サブカテゴリまたはプレイリストで非表示にするのではなく、コンテンツを非表示にしたり表示したりできます。</span><span class="sxs-lookup"><span data-stu-id="807a8-106">It offers a broader way to hide and show content than hiding it by subcategory or playlist.</span></span> <span data-ttu-id="807a8-107">たとえば、yammer サブカテゴリを非表示にすることはできますが、"yammer を使用して組織に接続する" など、特定のシナリオのプレイリストに yammer が表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="807a8-107">For example, you can hide a Yammer subcategory, but Yammer may still show up in certain scenario playlists such as "Connect your organization with Yammer".</span></span> <span data-ttu-id="807a8-108">特定のテクノロジがエンドユーザーに公開されないようにするには、テクノロジを使用して非表示にすることができます。</span><span class="sxs-lookup"><span data-stu-id="807a8-108">To ensure a specific technology is not exposed to end users, you can hide it by Technology.</span></span> 

## <a name="hide-a-technology"></a><span data-ttu-id="807a8-109">テクノロジを非表示にする</span><span class="sxs-lookup"><span data-stu-id="807a8-109">Hide a Technology</span></span>

1. <span data-ttu-id="807a8-110">カスタム学習**ホーム**ページから、 **Office 365 トレーニング**タイルをクリックします。</span><span class="sxs-lookup"><span data-stu-id="807a8-110">From the Custom Learning **Home** page, click the **Office 365 training** tile.</span></span>
2. <span data-ttu-id="807a8-111">カスタム学習 Web パーツで、[**システム**] メニューを選択し、[**プレイリストの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="807a8-111">From the Custom Learning Web part, select the **System** menu, then select **Administer Playlist**.</span></span> <span data-ttu-id="807a8-112">これで、2つのタブが表示されるようになります。</span><span class="sxs-lookup"><span data-stu-id="807a8-112">You should now have two tabs open.</span></span> <span data-ttu-id="807a8-113">1つは**カスタム学習管理**ページで、もう1つは**Office 365 トレーニング**ページです。</span><span class="sxs-lookup"><span data-stu-id="807a8-113">One with the **Custom Learning Administration** page, and one with the **Office 365 training** page.</span></span> 
3. <span data-ttu-id="807a8-114">**カスタム学習管理**ページで、**テクノロジ**をクリックし、そのテクノロジを非表示にする eyeball を選択します。</span><span class="sxs-lookup"><span data-stu-id="807a8-114">From the **Custom Learning Administration** page, click a **Technology**, and then select the eyeball for the Technology to hide it.</span></span> <span data-ttu-id="807a8-115">この例では、 **Yammer**テクノロジをクリックし、非表示にします。</span><span class="sxs-lookup"><span data-stu-id="807a8-115">For this example, click the **Yammer** technology, and then hide it.</span></span>  

![cg-hidetech](media/cg-hidetech.png)

### <a name="verify-the-playlist-is-hidden"></a><span data-ttu-id="807a8-117">再生リストが非表示になっていることを確認する</span><span class="sxs-lookup"><span data-stu-id="807a8-117">Verify the playlist is hidden</span></span>
1. <span data-ttu-id="807a8-118">**Yammer**テクノロジが非表示になっていることを確認するには、 **Office 365 トレーニング**ページが読み込まれたブラウザータブを選択して、ページを更新します。</span><span class="sxs-lookup"><span data-stu-id="807a8-118">To verify **Yammer** technology is hidden, select the browser tab with the **Office 365 training** page loaded, and then refresh the page.</span></span> <span data-ttu-id="807a8-119">Yammer のサブカテゴリが非表示になっていることがわかります。</span><span class="sxs-lookup"><span data-stu-id="807a8-119">You should now see the Yammer subcategory is hidden.</span></span> 
2. <span data-ttu-id="807a8-120">**推奨**サブカテゴリをクリックします。</span><span class="sxs-lookup"><span data-stu-id="807a8-120">Click the **Recommended** subcategory.</span></span> <span data-ttu-id="807a8-121">Yammer の [プレイリストを使用して組織を接続する」が非表示になっていることがわかります。</span><span class="sxs-lookup"><span data-stu-id="807a8-121">You'll notice that the Connect your organization with Yammer playlist is hidden.</span></span> 

![cg-hidetechrefresh](media/cg-hidetechrefresh.png)

## <a name="unhide-a-technology"></a><span data-ttu-id="807a8-123">テクノロジの表示/非表示</span><span class="sxs-lookup"><span data-stu-id="807a8-123">Unhide a Technology</span></span>

- <span data-ttu-id="807a8-124">[**カスタム学習管理**] ページで、[**テクノロジ**] の下の [テクノロジ] を選択し、非表示のテクノロジの eyeball を選択して非表示にします。</span><span class="sxs-lookup"><span data-stu-id="807a8-124">From the **Custom Learning Administration** page, under **Technology**, select a technology, then select the eyeball for the hidden technology to unhide it.</span></span> <span data-ttu-id="807a8-125">この例では、 **Yammer**テクノロジを再表示します。</span><span class="sxs-lookup"><span data-stu-id="807a8-125">For this example, unhide the **Yammer** technology.</span></span> 