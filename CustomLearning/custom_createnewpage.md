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
# <a name="create-sharepoint-pages-for-custom-playlists"></a>カスタム プレイリスト用の SharePoint ページの作成

学習経路のユニークな機能の 1 つは、Microsoft のアセットと作成した SharePoint アセットから組み立てられたプレイリストを作成する機能です。 この例では、プレイリストを作成する前に SharePoint ページを作成します。 SharePoint ページからプレイリストを作成する機能は、Microsoft または組織から利用可能な Web パーツを使用してページを作成するさまざまな機会を提供します。 たとえば、プレイリストには、YouTube の埋め込みビデオを含む SharePoint ページや、Office 365 フォームから作成されたフォーム、または埋め込み Power BI レポートを含めることができます。 この例では、埋め込み Web パーツとテキスト Web パーツを使用してページを作成する方法について説明します。  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>カスタム プレイリストの SharePoint ページを作成する

1. [SharePoint **Gear] アイコンを** クリックし、[ページの追加 **] をクリックします**。
2. ページ **の左側にある [新しいセクションの追加] (+)** をクリックし、セクション レイアウトの [2 つの **列** ] をクリックします。
3. 左側の列で、[+] をクリックし、[埋め込み] **Web パーツを** クリックします。 
4. 右側の列で、[+] をクリックし、[ **テキスト] Web パーツを** クリックします。 ページは次のように表示されます。

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>YouTube からビデオとテキストを追加する

1. ブラウザーで、YouTube に移動します。 この例では、"365 Office Microsoft の最高の生産性アプリ" を検索します。
2. ビデオをクリックして再生し、一時停止してから右クリックします。 
3. [埋 **め込みコードのコピー]** をクリックし、SharePoint ページに戻ります。 
4. [ **埋め込み] Web** パーツで **[埋** め込みコードの追加] をクリックし、YouTube ビデオからコードを追加します。
5. YouTube ページに戻り、ビデオの **説明テキスト** をコピーします。 
6. SharePoint ページに戻り、 **テキスト Web** パーツを選択し、YouTube ビデオからテキストをコピーします。
7. [SharePoint] **ページの [** タイトル] 領域で [Web パーツの編集] アイコンを選択し、[カスタム プレイリストの概要] ページに名前を付きます。 
8. [ **レイアウト] で**、[プレーン] **を** 選択し、[タイトル領域] プロパティ **ウィンドウ** を閉じます。 これで、ページは次のようになります。 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>ページを発行する

- [発行] **ボタンを選択** します。 これで、この SharePoint ページをカスタム プレイリストに追加する準備ができました。 