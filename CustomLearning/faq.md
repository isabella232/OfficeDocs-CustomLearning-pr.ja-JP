---
title: Microsoft 365 ラーニング パスに関するよく寄せられる質問
author: karuanag
ms.author: karuanag
ms.date: 02/10/2019
ms.topic: article
manager: alexb
audience: itpro
description: Microsoft 365 の学習経路に関するよく寄せられる質問の情報。
ms.service: sharepoint-online
ms.openlocfilehash: f791d6421740c3458be525a7e306b10edab58259
ms.sourcegitcommit: 96ad347dc08694ce2af5a5d42bf1f753d1c30a65
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749405"
---
# <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>最近、カスタム ラーニング for Office Microsoft 365 ラーニング パスに名前が変更されているというブログ投稿を見ました。 名前の変更作業の一環として、ソリューションに他の変更が追加されていますか? 組織のソリューションを更新する必要がありますか?

Microsoft 365 ラーニング パス リリースは、Microsoft 365 のブランド化に合わせてソリューションの名前を変更するためのブランド変更の取り組みです。 組織で現在 365 のカスタム Officeが正常に実行されている場合は、現時点でソリューションを更新する必要はありません。  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>テナント環境に Microsoft 365 ラーニング パスをインストールする場合の要件は何ですか?

- SharePoint Onlineとコミュニケーションサイトが有効になっています。
- CLO365 をプロビジョニングする個人は、インストール対象テナントのテナント管理者である必要があります。
- テナント 'App Catalog' は、SharePoint 管理センターの [アプリ] オプション内で使用できる必要があります。
- 新しいアプリ カタログを作成する場合、アプリ カタログを完全にプロビジョニングするには、30 分以上の待機時間が必要です。 テナント アプリ カタログの作成後に Microsoft 365 ラーニング パスを直接プロビジョニングしようとすると、ラーニング パス ソリューションのプロビジョニング エラーが発生します。 
- CLO365 をプロビジョニングする個人は、インストール対象テナントのアプリ カタログのサイト コレクション管理者である必要があります。

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Microsoft 365 ラーニング パスをインストールするときにテナントのアクセス許可を求める理由 

- SharePoint Online Provisioning サービスは、アクセス許可を使用して、ラーニング パスの SharePoint サイトをプロビジョニングし、サイトのページを作成し、テナント内に Microsoft 365 ラーニング パス アプリケーションをインストールします。 これは、アクセス許可を要求する唯一の理由です。 要求されたアクセス許可がない場合、SharePoint Provision Service は、学習経路サイト テンプレートと Web パーツを自動的にインストールするコマンドを実行できません。 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Microsoft 365 ラーニング パスがベータ プレビューに含めらどのような影響を受けるのか。 

Microsoft 365 のラーニング パスは現在ベータ プレビューに表示されています。 Microsoft 365 の学習経路を評価、計画、実装する際には、次の点を考慮してください。

- Beta ソリューションと同様に、サービス管理チームは、サービスとそのコンポーネントを変更する権利を持っています。 バグや UX の問題を積極的に解決する場合は、WebPart を更新する必要があります。
- Web パーツを更新するには、GitHub リポジトリから Web パーツをダウンロードし、テナント アプリ カタログにアップロードする必要があります。 Microsoft 365 ラーニング パス Readme ファイルの「ソリューションの更新」 [セクションを参照](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) してください。 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Microsoft 365 ラーニング パスは、どの言語で利用できますか?

Microsoft 365 ラーニング パスは現在、英語でのみ利用できます。 エンドツーエンドの自動プロビジョニングは、英語のテナントでのみ機能します。 2020 年第 2 四半期には、次の言語の多言語サポートを展開する予定です。 

- 中国語 (簡体字) 
- フランス語  
- ドイツ語 
- イタリア語 (イタリア) 
- 日本語 (日本)  
- ポルトガル語 (ブラジル) 
- ロシア語 (ロシア語)  
- スペイン語 

> オランダ語のサポートは、今後リリースされる学習経路の多言語サポートには含まれません。 今後も新しい言語オプションを評価していきます。

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>テナント環境にサイトをインストールするにはどのくらいの時間が必要ですか?

インストールのテストに基づいて、15 分未満かかる必要があります。 これには、要件に合わせてサイトをカスタマイズするために必要な時間は含まれません。

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 ラーニング パスはオープンソース ソリューションであり、どのような意味がありますか?

Microsoft 365 ラーニング パスは、オープンソース ソフトウェア (OSS) ソリューションであり、OSS に対する一連の利点と考慮事項を提供します。

#### <a name="benefits"></a>利点 
- **Microsoft 365 ラーニング パスは無料のソリューションです。** お客様は、テナントにソリューションをインストールし、カスタマイズし、エンド ユーザーがソリューションを利用できるようすることができます。
- **OSS を使用すると、迅速な開発とコラボレーションが可能です。**  すべてのオープンソース ソリューションは、幅広いコミュニティの投稿者が利用できます。  Microsoft は、イノベーションを推進するこの方法に取り組む。  お客様の最も幅広いセットに利益をもたらすエクスペリエンスを提供するために、コア サービス管理チームは、公式ビルドに組み込む投稿を決定する権利を持つ。  
- **OSS を使用すると、パートナーとの共同作業が可能です。** Microsoft は、複数のラーニング パートナーと協力して、Microsoft 365 ラーニング パスへの今後の拡張機能と貢献に向けた取り組みをサポートしています。 これらの計画が完了するに従って、より多くの情報を提供します。 
    
#### <a name="implications"></a>影響
- **OSS は市販の製品ではありません。** 商用製品には更新と修正プログラムが含まれており、有料サポート契約に含まれています。 Microsoft は現在、Microsoft 365 の学習経路に関するドキュメント、更新、修正プログラムを提供しますが、この特定のビジネス シナリオを改善する取り組みに基づいて行っています。 今後も、サービス管理チームが戦略を変更する可能性がある点に注意して、学習経路に投資し続ける予定です。 Microsoft 365 ラーニング パスに対する今後の変更は、有効になる前に伝達されます。 
- **OSS として、Microsoft 365** ラーニング パスは GitHub のオンラインの問題リストを通じてサポートされています。Microsoft 365 ラーニング パスは、既存の Microsoft サポート 契約ではカバーされません。 提出された問題は、Microsoft 365 ラーニング パスサービスの所有者とコミュニティによってトリアージされます。 問題解決サービス レベルは、有料の Microsoft サポート 契約と同じレベルではありません。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Microsoft 365 ラーニング パスをプライマリ SharePoint サイト コレクションのサブサイトにできますか?

いいえ。 サイトはコミュニケーション サイト テンプレートに基づいており、常にルート サイト コレクションを意味します。

> [!NOTE]
> エンド ユーザーがサイトにアクセスするために必要なアクセス許可を考慮することが重要です。 ほとんどの組織では、セキュリティ グループまたはユーザー グループが定義されています。 従業員コミュニティに起動する準備ができたら、適切なセキュリティ グループを新しいトレーニング ポータルに追加する必要があります。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>サイトを再インストールする必要があります。どうしたらいいでしょう。

ここに公開されているインストール手順に従 [います](custom_provision.md)。

> [!NOTE]
> 以前のインストールでテレメトリを無効にし、テレメトリを無効にして続行する場合は、ここでテレメトリを無効にする手順に従う必要があります。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Microsoft 365 ラーニング パスの実装に関する更新を行いました。 サイトを再インストールすると、これらの更新プログラム (サイト テンプレート、再生リスト) が失われるでしょうか。

現在のインストールでサイトを再インストールすると、個々のページとカスタム プレイリストのカスタマイズは失われます。  
