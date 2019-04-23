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
# <a name="create-sharepoint-pages-for-custom-playlists"></a>カスタムプレイリストの SharePoint ページを作成する

カスタム学習の固有の機能の1つとして、Microsoft や作成した SharePoint アセットから集められた再生リストを作成する機能があります。 この例では、再生リストを作成する前に SharePoint ページを作成します。 SharePoint ページからプレイリストを作成する機能は、Microsoft または組織から入手可能な Web パーツを使用してページを作成するさまざまな機会を提供します。 たとえば、リストには、YouTube からのビデオが埋め込まれた SharePoint ページ、Office 365 フォームから作成されたフォーム、または組み込み Power BI レポートを含めることができます。 この例では、埋め込み web パーツとテキスト web パーツを使用してページを作成する方法を示します。  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>カスタムプレイリストの SharePoint ページを作成する

1. SharePoint**歯車**アイコンをクリックし、[**ページの追加**] をクリックします。
2. ページの左側にある [**新しいセクションの追加] (+)** をクリックし、[セクションレイアウト] で [ **2 列**] をクリックします。
3. 左側の列で、[+] をクリックし、[**埋め込み**web パーツ] をクリックします。 
4. 右の列で、[+] をクリックし、[**テキスト**web パーツ] をクリックします。 ページは次のようになります。

![cg-pagenewstart](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>YouTube からのビデオおよびテキストの追加

1. ブラウザーで、[YouTube] に移動します。 この例では、「Office 365 – Microsoft のベストプロダクティビティアプリ」を検索します。
2. ビデオをクリックして再生し、一時停止して、それを右クリックします。 
3. [**埋め込みコードのコピー**] をクリックし、SharePoint ページに戻ります。 
4. **埋め込み**web パーツで [**埋め込みコードの追加**] をクリックし、YouTube ビデオからコードを追加します。
5. [YouTube] ページに戻り、ビデオの**説明**テキストをコピーします。 
6. SharePoint ページに戻り、**テキスト**web パーツを選択してから、YouTube ビデオからテキストをコピーします。
7. SharePoint ページのタイトル領域で [ **web パーツの編集**] アイコンを選択し、そのページに「Custom プレイリストの紹介」という名前を指定します。 
8. [**レイアウト**] で、[**プレーン**] を選択し、[**タイトル領域**のプロパティ] ウィンドウを閉じます。 これで、ページは次のように表示されます。 

![cg-pagenewfinish](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>ページの発行

- [**発行**] ボタンを選択します。 これで、この SharePoint ページをカスタムプレイリストに追加する準備ができました。 