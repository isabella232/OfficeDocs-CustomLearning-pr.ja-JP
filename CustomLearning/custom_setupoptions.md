---
author: pkrebs
ms.author: pkrebs
title: 学習経路のセットアップ オプション
ms.date: 07/16/2020
description: 学習経路のセットアップ オプション
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 2397f7930bcf02ed697dcc6b18b648bffa2f0e11
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000333"
---
# <a name="configuration-options-for-multilingual-learning-pathways"></a>多言語学習経路の構成オプション
SharePoint Online コミュニケーション サイトの多言語機能がリリースされたので、学習パスは複数の言語のサポートを提供しています。 組織のニーズを満たすために、さまざまな方法で学習経路を設定できます。 組織に最適なパスを決定するために、セットアップ オプションの概要を説明しました。 

## <a name="new-install-scenarios"></a>新しいインストール シナリオ
「新しいインストール シナリオ」では、Microsoft 365 ルックブック サービスを使用して学習経路の新しいインスタンスをインストールするためのオプションについて説明します。 

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>シナリオ 1: 学習パスをインストールしていないので、多言語サポートの学習パスが必要です 
ラーニング パスをインストールしていないのに複数の言語が必要な場合は、Microsoft 365 のルック ブック サービスを使用して、9 つの言語をサポートする新しい学習経路ソリューションをインストールできます。 英語は既定の言語であり、変更できません。 
- サイトの既定の言語として英語で新しい学習経路ソリューションをプロビジョニングするには、「新しい学習経路ソリューションを準備する [」を参照してください](custom_provision.md)。

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>シナリオ 2: 学習パスはインストールされましたが、現在使用していないか、サイトまたはプレイリストのカスタマイズを行っていない 
学習パスをインストールしたが、アクティブに使用していない場合、またはサイトやプレイリストをカスタマイズしていない場合は、Microsoft 365 のルック ブック サービスを使用して、9 つの言語をサポートする新しいソリューションをインストールできます。 英語は既定の言語であり、変更できません。 
- サイトの既定の言語として英語で新しい学習経路ソリューションをプロビジョニングするには、「新しい学習経路ソリューションを準備する [」を参照してください](custom_provision.md)。

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>シナリオ 3: 学習経路がインストールされていないので、多言語サポートは必要ない 
ラーニング パスをインストールしていないのに多言語サポートが必要ない場合は、Microsoft 365 ルック ブック サービスからインストールできます。 英語は既定の言語になります。 インストール後、多言語サポートをオフにする必要があります。 
- 多言語サポートなしで新しい学習経路ソリューションを準備するには、「新しい学習経路ソリューションを準備 [する」を参照してください](custom_provision.md)。

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>学習経路を更新する (Web パーツのアップロードを使用して) シナリオ
既存のバージョンのラーニング パスがインストールされている場合は、ラーニング パス Web パーツを SharePoint アプリ カタログにアップロードして多言語サポートを有効にできます。 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>シナリオ 1: 既存のバージョンの学習パスをアップグレードする必要がありますが、多言語サポートは必要ない
多言語サポートなしで、学習経路バージョン 4.0 を更新できます。 この更新プログラムでは、カスタムプレイリストやサブカテゴリのイメージ セレクターなど、いくつかの新機能を利用できます。 

- 多言語サポートなしで既存の学習経路ソリューションを更新するには、「多言語サポートのための学習経路の更新 [」を参照してください](custom_update.md)。 多言語サポートのアップグレード プロセスは、多言語サポートと同じですが、手順は少なめです。 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>シナリオ 2: 多言語サポートにアップグレードする必要があります。サイト コレクションの既定の言語は既定の言語です
ラーニング パス バージョン 4.O は、サイト コレクション内の多言語ページをサポートします。 多言語サポートに加えて、カスタム プレイリストやサブカテゴリのイメージ セレクターなど、いくつかの新機能が追加されています。 
- 既存のラーニング パス サイトの多言語サポートを更新するには、「多言語サポート用の学習パスを [更新する」を参照してください](custom_update.md)。 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>手動インストールを使用して多言語サポートの学習経路を更新する 
次に、ラーニング パス Web パーツを手動でインストールして、ラーニング パス ソリューションの既存のインスタンスをバージョン 4.0 多言語バージョンに更新するシナリオの概要を示します。 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>シナリオ 1: 多言語サポートが必要で、サイト コレクションの既定の言語は既定の言語ではなく、カスタム コンテンツはありません 
ラーニング パス バージョン 4.0 は、このシナリオをサポートします。 ただし、このシナリオでは、既存のサイトにカスタム コンテンツやプレイリストが含まれるとは想定されません。 このシナリオでは、既定の言語で新しい SharePoint Online 通信サイトを作成し、Web パーツをアップロードしてから、PowerShell スクリプトを使用して手動で学習経路を設定できます。 
- 既定の言語で多言語サポート用の学習パスを設定するには、「多言語サポート用のラーニング パスの手動インストール」 [を参照してください](custom_manualsetup.md)。

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>シナリオ 2: 多言語サポートが必要で、サイト コレクションの既定の言語が既定の言語ではなく、カスタム コンテンツがある 
このシナリオでは、既定の言語で新しい SharePoint Online 通信サイトを作成し、Web パーツをアップロードしてから、PowerShell スクリプトを使用して手動で学習経路を設定できます。 

上記の手順に従って学習パス サイトを再確立した後 **、CustomPlaylists** リストと CustomAssets リストの内容を **移動する必要** があります。 また、必要に応じて、カスタム アセットを構成する実際のカスタム ページを、既存の学習経路サイトに住んでいる場合に移動し、そのページを削除する目的で移動することもできます。 **CustomPlaylists** リスト内のすべてのアイテムに対して **、CustomAssets** リスト内のリスト アイテムの ID が各プレイリスト リスト アイテムの JSONData フィールドに埋もれているため、タスクが困難になる可能性があります。 したがって **、CustomPlaylists** リストのコンテンツをあるサイトから別のサイトに移動するだけでは十分ではありません。 さらに **、CustomAssets リスト** には、リスト アイテムの JSONData フィールドにあるカスタム アセットのページへの絶対 URL が含まれる。 アセットが移動され、サイトの名前が変更されない場合 (したがって、絶対 URL をアセットのページに変更 **)、CustomAssets はそのまま** 残ります。 ただし、エントリを手動で修正する必要があります。 移行のこの種類の複雑さを考えると、この移行を支援するために、学習経路パートナーの 1 つを参加させる方法を検討してください。
- 既定の言語で多言語サポート用の学習パスを設定するには、「多言語サポート用のラーニング パスの手動インストール」 [を参照してください](custom_manualsetup.md)。