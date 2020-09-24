---
author: pkrebs
ms.author: pkrebs
title: 経路管理の学習
ms.date: 02/15/2019
description: Web パーツまたはメニューからカスタム学習管理ページにアクセスする方法
ms.service: sharepoint online
ms.openlocfilehash: b491c0416573ddf3be6cda3afc8182cdc746649d
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233329"
---
# <a name="access-the-learning-pathways-administration-page"></a><span data-ttu-id="3748b-103">ラーニング経路管理ページにアクセスする</span><span class="sxs-lookup"><span data-stu-id="3748b-103">Access the Learning Pathways Administration page</span></span>

<span data-ttu-id="3748b-104">ラーニングの経路管理は、CustomLearningAdmin ページから管理されます。</span><span class="sxs-lookup"><span data-stu-id="3748b-104">Learning pathways administration is managed from the CustomLearningAdmin.aspx page.</span></span> <span data-ttu-id="3748b-105">この管理ページは、SharePoint 管理者のみが使用できます。</span><span class="sxs-lookup"><span data-stu-id="3748b-105">This administration page is only available to SharePoint Administrators.</span></span> <span data-ttu-id="3748b-106">サイトを訪問するメンバー権限を持つユーザーには、Web パーツの **管理** 歯車アイコンは表示されません。</span><span class="sxs-lookup"><span data-stu-id="3748b-106">Users with member privileges visiting the site will not see the **Administration** gear icon on the Web part.</span></span> <span data-ttu-id="3748b-107">さらに、管理者のみが、SharePoint**ホーム**メニューの [**ラーニングパス] 管理**メニュー項目から管理ページを開くことができます。</span><span class="sxs-lookup"><span data-stu-id="3748b-107">In addition, only Administrators will have the ability to open the administration page from the **Learning pathways administration** menu item under the SharePoint **Home** menu.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="3748b-108">製品のサブカテゴリまたは再生リストを非表示にするなど、カスタム学習管理ページで行われた変更は、Web パーツのすべてのインスタンスに反映されます。</span><span class="sxs-lookup"><span data-stu-id="3748b-108">Changes made on the Custom Learning Administration page, such as hiding a product subcategory or playlist, will be reflected in all instances of the Web part.</span></span> <span data-ttu-id="3748b-109">さらに、複数のユーザーが同時にページを使用している場合は、カスタム学習では競合を検出できないため、管理ページから変更を加えることができるのは1人の管理者のみにすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3748b-109">In addition, it’s recommended that only one administrator at time make changes from the administration page, since Custom Learning does not provide collision detection if multiple people are using the page at the same time.</span></span>  

## <a name="access-from-the-learning-pathways-web-part---preferred-method"></a><span data-ttu-id="3748b-110">学習経路 web パーツからのアクセス-推奨される方法</span><span class="sxs-lookup"><span data-stu-id="3748b-110">Access from the Learning pathways web part - preferred method</span></span>
<span data-ttu-id="3748b-111">Web パーツから管理ページを開くことは、そのページを新しいブラウザータブで開くために推奨される方法です。このメソッドを使用すると、タブ付きページ間を前後にめくって作業をチェックしたり、変更したりするのは簡単です。</span><span class="sxs-lookup"><span data-stu-id="3748b-111">Opening the Administration page from the web part is the preferred method since it opens the page in a new browser tab. With this method, it's easy to flip back and forth between the tabbed pages to check or modify your work.</span></span>  

1. <span data-ttu-id="3748b-112">Microsoft 365 learning の経路の **ホーム** ページから、 **Office 365 のトレーニング** タイルをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3748b-112">From the Microsoft 365 learning pathways **Home** page, click the **Office 365 training** tile.</span></span>
2. <span data-ttu-id="3748b-113">次の例に示されているように、Web パーツの [ **管理** ] アイコンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3748b-113">Click the **Administration** icon in the Web part as shown in the following example</span></span>  

![cg-adminaccbtn.png](media/cg-adminaccbtn.png)

## <a name="access-from-the-home-menu-item"></a><span data-ttu-id="3748b-115">ホームメニュー項目からのアクセス</span><span class="sxs-lookup"><span data-stu-id="3748b-115">Access from the Home menu item</span></span>
<span data-ttu-id="3748b-116">管理者は、Web パーツを含むページに移動するのではなく、SharePoint **ホーム** メニューの項目から管理ページにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3748b-116">Rather than navigate to a page with a Web part, administrators can access the Adminstration page from the SharePoint **Home** menu item.</span></span> 

- <span data-ttu-id="3748b-117">Microsoft 365 Learning の経路のホームページで、[ **ホーム** ] メニューをクリックし、[ **Microsoft Learning administration**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3748b-117">From the Microsoft 365 Learning Pathways Home page, click the **Home** menu, then click **Microsoft learning administration**.</span></span>

![cg-adminaccmenu.png](media/cg-adminaccmenu.png)