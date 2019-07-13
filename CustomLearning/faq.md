---
author: karuanag
ms.author: karuanag
title: Microsoft 365 学習経路のよく寄せられる質問
ms.date: 02/10/2019
description: Microsoft 365 学習経路のよく寄せられる質問情報
ms.openlocfilehash: 66149439f0ca13b319bee3bea9c2773b43e98e25
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35636111"
---
# <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>最近、ブログ投稿が公開されました。 Office 365 のカスタム学習は、Microsoft 365 Learning の経路に変更されています。 名前の変更作業の一環として、ソリューションに他の変更が追加されているかどうか。 組織内のソリューションを更新する必要がありますか。

Microsoft 365 learning の経路のリリースは、Microsoft 365 ブランド化に合わせてソリューションの名前を変更することに特化した rebranding 努力です。 組織内で現在正常に実行されている Office 365 のカスタム学習がある場合、現時点ではソリューションを更新する必要はありません。  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Microsoft 365 learning の経路をテナント環境にインストールするための要件は何ですか。

- SharePoint Online とコミュニケーションサイトが有効になっている。
- CLO365 をプロビジョニングするユーザーは、インストール先のテナントのテナント管理者である必要があります。
- テナント ' App Catalog ' は、SharePoint 管理センターの [アプリ] オプション内で使用できる必要があります。
- 新しいアプリカタログが作成された場合、アプリカタログを完全にプロビジョニングするには、30分以上の待機時間が必要になります。 テナントのアプリカタログを作成した後で、Microsoft 365 learning の経路を直接プロビジョニングしようとすると、ラーニングパスソリューションのプロビジョニングエラーが発生します。 
- CLO365 をプロビジョニングするユーザーは、インストール先のテナントのアプリカタログのサイトコレクション管理者である必要があります。

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Microsoft 365 learning の経路をインストールするときに Microsoft がテナントのアクセス許可を要求する理由 

- SharePoint Online プロビジョニングサービスは、アクセス許可を使用して、ラーニングパス SharePoint サイトをプロビジョニングし、サイトのページを作成し、テナント内に Microsoft 365 Learning のパスアプリケーションをインストールします。 これは、アクセス許可を要求する唯一の理由です。 要求されたアクセス許可がないと、SharePoint プロビジョニングサービスは、学習経路サイトテンプレートと web パーツを自動的にインストールするコマンドを実行できません。 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>ベータ版のプレビューには、Microsoft 365 の学習経路がどのような影響がありますか。 

Microsoft 365 の学習経路は、現在ベータ版のプレビューに含まれています。 Microsoft 365 learning の経路を評価、計画、および実装する際には、次の点を考慮してください。

- 任意のベータソリューションと同様に、サービス管理チームはサービスとそのコンポーネントに変更を加える権利を留保します。 バグと UX の問題を解決している間は、Web パーツを更新する必要があります。
- Web パーツを更新するには、GitHub リポジトリからダウンロードして、テナントのアプリカタログにアップロードする必要があります。 「Microsoft 365 learning の[Readme](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)ファイル」の「ソリューションを更新する」セクションを参照してください。 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Microsoft 365 の学習経路はどの言語で利用できますか?

現在、Microsoft 365 の学習経路は英語でのみご利用いただけます。 自動エンドツーエンドプロビジョニングは、英語のテナントでのみ機能します。 CY19 Q4 では、次の9つの言語について多言語サポートをロールアウトすることを計画しています。 

- 簡体字中国語 
- オランダ語 (オランダ) 
- フランス語  
- ドイツ語 
- イタリア語 (イタリア) 
- 日本語 (日本)  
- ポルトガル語 (ブラジル) 
- ロシア語 (ロシア)  
- スペイン語 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>テナント環境にサイトをインストールするには、どのくらいの時間がかかりますか?

インストールのテストに基づき、15分未満で完了する必要があります。 これには、要件に合わせてサイトをカスタマイズするのに必要な時間は含まれません。

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 learning はオープンソースソリューションに影響を与えますか?

Microsoft 365 learning の経路は、Open Source Software (OSS) ソリューションであり、次のような一連の利点と考慮事項が germane にあります。

#### <a name="benefits"></a>利点 
- **Microsoft 365 学習経路は無料のソリューションです。** お客様は、お客様のテナントにソリューションをインストールし、カスタマイズしてエンドユーザーが使用できるようにすることができます。
- **OSS は、迅速な開発とコラボレーションを可能にします。** すべてのオープンソースソリューションは、投稿者の広範なコミュニティで利用できます。  Microsoft は、技術革新を推進するためにこの方法をコミットしています。  お客様の主要なサービス管理チームが、お客様の正式な構築にどのような貢献が組み込まれているかを判断するための適切な経験を提供することにより、お客様にメリットがもたらされます。  
- **OSS はパートナーとの共同作業を可能にします。** Microsoft は、今後の拡張および Microsoft 365 learning 経路への貢献に向けた取り組みをサポートするために、いくつかの学習パートナーと連携しています。 これらのプランが最終処理されるときに、詳細情報を提供します。 
    
#### <a name="implications"></a>関連
- **OSS は、市販の製品ではありません。** 商用製品には、更新と修正プログラムが含まれており、料金ベースのサポート契約に含まれています。 Microsoft は現在、Microsoft 365 learning の経路に関するドキュメント、更新、パッチを提供していますが、この特定のビジネスシナリオを改善するための取り組みに基づいています。 このプランでは、学習経路への投資を継続することになりますが、お客様は、サービス管理チームが将来的に戦略を変更する可能性があることに注意する必要があります。 今後の Microsoft 365 learning 経路への変更は、有効になる前に伝達されます。 
- **OSS では、microsoft 365 の学習経路は、GitHub のオンライン問題リストを通じてサポート**されます。 microsoft 365 learning の経路は、既存の microsoft サポート契約の対象外です。 提出された問題には、Microsoft 365 learning のサービス所有者とコミュニティによるトリアージがあります。 問題解決サービスレベルは、有償の Microsoft サポート契約と同じレベルではありません。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Microsoft 365 learning は、プライマリ SharePoint サイトコレクションのサブサイトを作成できますか。

いいえ。 サイトは、コミュニケーションサイトテンプレートに基づいています。これは、常にルートサイトコレクションであることを意図しています。

> [!NOTE]
> エンドユーザーがサイトにアクセスするために必要なアクセス許可について考慮することが重要です。 多くの組織では、セキュリティまたはユーザーグループを定義しています。 従業員コミュニティに対してを開始する準備ができたら、適切なセキュリティグループを新しいトレーニングポータルに追加する必要があります。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>サイトを再インストールする必要があります。どうしたらいいでしょう。

[ここで](custom_provision.md)公開されているインストール手順に従います。

> [!NOTE]
> 以前のインストールでテレメトリを無効にしていて、テレメトリを無効にしたままにする場合は、ここでテレメトリを無効にするための手順に従う必要があります。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Microsoft 365 の学習経路の実装に対して更新を行いました。 サイトを再インストールすると、これらの更新プログラム (サイトテンプレート、再生リストに加えられたもの) は失われますか?

現在のインストール環境でサイトを再インストールすると、個々のページおよびカスタム再生リストに対するカスタマイズが失われます。  