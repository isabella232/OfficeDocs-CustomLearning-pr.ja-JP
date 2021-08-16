---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学習経路をアップデートする
ms.date: 07/06/2020
description: Microsoft 365 学習経路をアップデートする
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: daea2e2880c47a2ba5d961338e4f6d04c23b8e99
ms.sourcegitcommit: 152e8d7489c80beeb7d9ebfd04e6ef8ec7aed454
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2021
ms.locfileid: "58350595"
---
# <a name="update-learning-pathways"></a>学習経路を更新する
既存のパスウェイ サイトラーニング場合は、多言語サポート用に更新できます。 多言語 4.0 バージョンへの学習パスを更新するには、web パーツ パッケージ customlearning.sppkg をテナントアプリ カタログSharePointアップロードします。 学習経路を更新する場合:  

- 以前に作成されたカスタムプレイリストとアセットは維持されます
- 設定を非表示または表示する機能が維持される
- テンプレートの学習SharePointは変更されません
- 学習経路サイト ページは翻訳されません。 この作業は手動で行う必要があります

## <a name="read-the-learning-pathways-multilingual-overview"></a>多言語の学習経路の概要を読む
多言語サポートが学習経路でどのように機能するのかについては、「多言語ラーニング[の概要」を参照してください](custom_overview.md)。 

## <a name="prerequisites-to-update"></a>更新の前提条件
学習経路を更新する前に、次の前提条件を満たしている必要があります。
- ラーニング パスを更新するユーザーは、テナント アプリ カタログのサイト コレクション所有者である必要があります。 ユーザープロビジョニング学習パスがアプリ カタログのサイト コレクション所有者ではない場合は、次の手順 [を実行](addappadmin.md) して続行します。 

## <a name="set-language-settings"></a>言語設定の設定 
学習経路を更新する前に、サイトの言語設定を設定します。 ラーニング パス サイトの多言語サポートを有効にするには、[ページとニュースを複数の言語に翻訳するを有効にする] を **[オン**] に設定し、サイトでサポートする言語を追加できます。
1.  [パスラーニング] サイトで、設定 **から**[サイト情報] を **選択します**。
2.  サイト情報ウィンドウの下部で、[すべてのサイト設定を表示 **する] を選択します**。
3.  [サイト **の管理] で**、[言語の **設定] を選択します**。
4.  [ **複数の言語に翻訳する** ページとニュースを有効にする] で、トグル スイッチを設定します。 
- 複数のサイトの場合は、トグルを **[オン**] にスライドし、[言語の追加] セクションに進みます。 
- 英語専用サイトの場合は、トグルを Off にスライド **します**。

### <a name="add-languages"></a>言語を追加する
ラーニング 9 つの言語がサポートされている場合は、必要な言語のみを追加する必要があります。 このドキュメントで使用されている例では、イタリア語が追加されます。 
- [**サイト言語の追加と** 削除] で、[言語の選択または入力] で言語名の入力を開始するか、ドロップダウンから言語を選択します。 この手順を繰り返して、複数の言語を追加できます。 このページに戻って、いつでもサイトの言語を追加または削除できます。
 
### <a name="assign-translators"></a>翻訳者の割り当て
学習経路の言語設定を定義する場合は、翻訳者を割り当てできます。 翻訳者には外国語プロファイルが設定されている必要があります。 外国語プロファイルの詳細については、「多言語コミュニケーション サイト、ページ、ニュースを作成する [」を参照してください](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。  
- サポートされている言語の場合は、[選択] **をクリックするか、翻訳者を入力** し、翻訳者を選択します。 

## <a name="update-the-learning-pathways-web-part-package"></a>ラーニング パス Web パーツ パッケージを更新する
この手順では、学習パス 4.0 Web パーツを SharePoint アプリ カタログにアップロードし、[学習経路の管理] ページに移動して更新プロセスを開始します。

### <a name="upload-the-web-part-package"></a>アップロードパーツ パッケージの作成
- Web パーツの更新に関する最新の情報については、「README ラーニング[を参照してください](https://github.com/pnp/custom-learning-office-365#updating-the-solution)。 

### <a name="next-steps"></a>次の手順
- サイトと [Web パーツで提供](custom_exploresite.md) される既定のコンテンツを確認します。
- サイト ページの翻訳の詳細については、「サイト ページの翻訳 [」を参照してください](custom_translate_page_ml.md)。 

