---
author: pkrebs
ms.author: pkrebs
title: ラーニング経路のセットアップオプション
ms.date: 07/16/2020
description: ラーニング経路のセットアップオプション
ms.openlocfilehash: 1434a06fbe5f374de7b2f2e4fa471a8eda5ac871
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.contentlocale: ja-JP
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043219"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>多言語学習経路のセットアップオプション
SharePoint Online コミュニケーションサイトの多言語機能のリリースにより、複数言語のサポートが提供されるようになりました。 さまざまな方法で学習経路を設定して、組織のニーズを満たすことができます。 組織にとって最適なパスを決定するのに役立つように、セットアップオプションの概要を説明しました。 

## <a name="new-install-scenarios"></a>新しいインストールシナリオ
「新しいインストールシナリオ」では、Microsoft 365 look book サービスを使用して、ラーニング経路の新しいインスタンスをインストールするためのオプションについて説明します。 

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>シナリオ 1: 学習経路がインストールされておらず、学習経路の多言語サポートが必要である 
学習経路がインストールされておらず、複数の言語が必要な場合は、Microsoft 365 look book サービスを使用して、9つの言語をサポートする新しいラーニングパスソリューションをインストールすることができます。 英語は既定の言語で、変更することはできません。 
- サイトの既定の言語として英語を使用して新しい学習経路ソリューションを準備するには、「[新しい学習経路ソリューションを準備](custom_provision.md)する」を参照してください。

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>シナリオ 2: 学習経路をインストールしましたが、現在は使用していないか、サイトまたはプレイリストをカスタマイズしていません 
学習経路をインストールしたが、それをアクティブに使用していない場合、またはサイトまたはプレイリストに対してカスタマイズを行っていない場合は、Microsoft 365 look book service を使用して、9つの言語をサポートする新しいソリューションをインストールすることができます。 英語は既定の言語で、変更することはできません。 
- サイトの既定の言語として英語を使用して新しい学習経路ソリューションを準備するには、「[新しい学習経路ソリューションを準備](custom_provision.md)する」を参照してください。

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>シナリオ 3: 学習経路をインストールしておらず、多言語サポートを必要としない 
学習経路をインストールしておらず、多言語サポートを必要としない場合は、Microsoft 365 look book service からインストールできます。 英語は既定の言語になります。 インストール後、多言語サポートを無効にする必要があります。 
- 多言語サポートなしで新しい学習経路ソリューションを準備するには、「[新しい学習経路ソリューションを準備](custom_provision.md)する」を参照してください。

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>学習経路を更新する (web パーツのアップロードを使用した場合)
既存のバージョンの学習機能がインストールされている場合は、ラーニング経路 web パーツを SharePoint アプリカタログにアップロードして、多言語サポートを有効にすることができます。 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>シナリオ 1: 学習経路の既存バージョンをアップグレードする必要があるが、多言語サポートは必要ない
多言語サポートがない場合は、ラーニング経路バージョン4.0 を更新できます。 この更新プログラムを使用すると、カスタムの再生リストおよびサブカテゴリのイメージセレクターを含む、いくつかの新機能を利用できます。 

- 多言語サポートのない既存の学習経路ソリューションを更新する方法については、「[多言語サポートのための学習経路を更新](custom_update.md)する」を参照してください。 多言語サポートのアップグレードプロセスは、多言語サポートの場合と同じですが、手順は少なくなります。 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>シナリオ 2: 多言語サポートへのアップグレードが必要で、サイトコレクションの既定の言語が既定の言語である
ラーニング経路バージョン4は、サイトコレクション内の多言語ページをサポートします。 多言語サポートに加えて、カスタムの再生リストやサブカテゴリのイメージセレクターを含む、いくつかの新機能を利用できます。 
- 既存の学習経路サイトの多言語サポートを更新するには、[多言語サポートのための学習経路の更新](custom_update.md)を参照してください。 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>手動インストールを使用した多言語サポートの学習経路を更新する 
次に示すのは、学習機能の web パーツを手動でインストールすることによって、ラーニングパスソリューションの既存のインスタンスをバージョン4.0 の多言語バージョンに更新するシナリオの概要です。 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>シナリオ 1: 多言語のサポートが必要であり、サイトコレクションの既定の言語が既定の言語ではない (カスタムコンテンツを持たない) 
ラーニング・経路バージョン4.0 はこのシナリオをサポートします。 ただし、このシナリオでは、既存のサイトにカスタムコンテンツまたはプレイリストがないことを前提としています。 このシナリオでは、既定の言語を使用して新しい SharePoint Online コミュニケーションサイトを作成し、web パーツをアップロードしてから、PowerShell スクリプトを使用して学習経路を手動で設定することができます。 
- 多言語サポートのための学習経路を既定の言語で設定するには、「[多言語サポートのための学習経路の手動インストール](custom_manualsetup.md)」を参照してください。

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>シナリオ 2: 多言語のサポートが必要であり、サイトコレクションの既定の言語が既定の言語ではなく、さらにカスタムコンテンツを持っている 
このシナリオでは、既定の言語を使用して新しい SharePoint Online コミュニケーションサイトを作成し、web パーツをアップロードしてから、PowerShell スクリプトを使用して学習経路を手動で設定することができます。 

上記の手順に従って学習機のサイトを再確立した後、 **Customplaylists**リストのリストと**customplaylists**リストの内容を移動する必要があります。 また、必要に応じて、カスタムアセットを構成する実際のカスタムページを既存の学習機能サイトにある場合は、それらを削除することもできます。 **Customplaylists**リスト内のすべてのアイテムに対して、 **customplaylists**リスト内のリストアイテムの ID が、各再生リストのリストアイテムの jsondata フィールドに埋め込まれているため、タスクが困難になることがあります。 したがって、あるサイトから別のサイトに**Customplaylists**リストのコンテンツを移動するだけでは不十分です。 さらに、 **Customassets**リストには、リストアイテムの jsondata フィールドにカスタムアセットのページへの絶対 URL が含まれています。 アセットが移動されず、サイトの名前が変更されない (つまり、絶対 URL がアセットのページに変更される) 場合、 **Customassets**を残すことができます。 ただし、エントリを手動で修正する必要があります。 この種類の移行の複雑さを考慮して、この移行を支援するために、ラーニング経路パートナーの1つを参加させることをお勧めします。
- 多言語サポートのための学習経路を既定の言語で設定するには、「[多言語サポートのための学習経路の手動インストール](custom_manualsetup.md)」を参照してください。