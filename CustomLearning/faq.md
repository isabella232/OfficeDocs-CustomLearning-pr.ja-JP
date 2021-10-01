---
title: Microsoft 365学習パスに関する FAQ
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: 学習経路に関するよく寄せられるMicrosoft 365情報
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 82a7e777490e13fde6fef5add40beee417050027
ms.sourcegitcommit: d05381fc4a58cf2949773d73877bacc5ef3a7ca6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/01/2021
ms.locfileid: "60048724"
---
# <a name="frequently-asked-questions"></a>よく寄せられる質問

## <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>テナント環境に学習経路をインストールMicrosoft 365要件は何ですか?

- SharePoint Onlineとコミュニケーションサイトが有効になっています。
- 学習経路をプロビジョニングするMicrosoft 365は、インストール対象テナントのテナント管理者である必要があります。
- テナント 'App Catalog' は、管理センターの [アプリ] オプション内SharePoint必要があります。
- 新しいアプリ カタログを作成する場合、アプリ カタログを完全にプロビジョニングするには、30 分以上の待機時間が必要です。 テナント アプリ カタログMicrosoft 365後に直接、学習パスをプロビジョニングしようとすると、学習経路ソリューションのプロビジョニング エラーが発生します。
- ラーニング パスをプロビジョニングするMicrosoft 365は、インストール対象テナントのアプリ カタログのサイト コレクション管理者である必要があります。

## <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Microsoft がラーニング パスをインストールするときにテナントのアクセス許可を求Microsoft 365理由

SharePoint Online Provisioning サービスは、アクセス許可を使用して ラーニング Pathways SharePoint サイトをプロビジョニングし、サイトのページを作成し、Microsoft 365 ラーニング パスウェイ アプリケーションをテナント内にインストールします。 これは、アクセス許可を要求する唯一の理由です。 要求されたアクセス許可がない場合、SharePoint サービスは、学習経路サイト テンプレートと Web パーツを自動的にインストールするコマンドを実行できません。
![アクセス許可要求のスクリーンショット](media/faqs-permissions-request-screenshot.png "アクセス許可の要求") このレベルのアクセスについて引き続き懸念がある場合は、アクセス許可を付与し、関心のあるサイト テンプレートを展開し、付与されたアクセス許可を Azure アプリ ストアのアプリに直ちに [削除できます](https://myapps.microsoft.com)。

## <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>テナント環境にサイトをインストールするにはどのくらいの時間が必要ですか?

15 分未満の時間が必要です。 これには、要件に合わせてサイトをカスタマイズするために必要な時間は含まれません。

## <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>学習Microsoft 365はオープンソース ソリューションであり、どのような意味がありますか?

Microsoft 365学習経路は、オープンソース ソフトウェア (OSS) ソリューションであり、OSS に対する一連の利点と考慮事項を提供します。

### <a name="benefits"></a>利点 

- **Microsoft 365学習経路は無料のソリューションです。** 顧客は、ソリューションをテナントにインストールし、カスタマイズし、エンド ユーザーが利用できるようすることができます。
- **OSS を使用すると、迅速な開発とコラボレーションが可能です。** すべてのオープンソース ソリューションは、幅広いコミュニティの投稿者が利用できます。 Microsoft は、イノベーションを推進するこの方法に取り組む。 お客様の幅広いセットにメリットをもたらすエクスペリエンスを提供するために、コア サービス管理チームは、公式ビルドに組み込む投稿を決定する権利を持っています。  
- **OSS を使用すると、パートナーとの共同作業が可能です。** Microsoft は、複数の学習パートナーと協力して、将来の拡張機能や学習経路への貢献に対する取り組みをMicrosoft 365しています。 これらの計画が完了するに従って、より多くの情報を提供します。

### <a name="implications"></a>影響

- **OSS は市販の製品ではありません。** 商用製品には更新と修正プログラムが含まれており、有料サポート契約に含まれています。 Microsoft は現在、学習経路に関するドキュメント、更新、修正プログラムを提供Microsoft 365、この特定のビジネス シナリオを改善する取り組みに基づいて行っています。 学習経路への投資を継続する予定ですが、サービス管理チームは将来戦略を変更する可能性があります。 将来の学習経路Microsoft 365変更は、有効になる前に伝達されます。
- **OSS として、Microsoft 365** ラーニング パスは GitHub : Microsoft 365 ラーニング パスのオンラインの問題リストを通じてサポートされます。既存の Microsoft サポート 契約ではサポートされていません。 提出された問題は、サービスMicrosoft 365コミュニティの学習経路によってトリアージされます。 問題解決サービス レベルは、有料の Microsoft サポート 契約と同じレベルではありません。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-sub-site-of-our-primary-sharepoint-site-collection"></a>学習経路をMicrosoft 365サイト コレクションのサブサイトSharePointできますか?

その必要はありません。 サイトはコミュニケーション サイト テンプレートに基づいており、常にルート サイト コレクションを意味します。

> [!NOTE]
> エンド ユーザーがサイトにアクセスするために必要なアクセス許可を考慮することが重要です。 ほとんどの組織では、セキュリティ グループまたはユーザー グループが定義されています。 従業員コミュニティに起動する準備ができたら、適切なセキュリティ グループを新しいトレーニング ポータルに追加する必要があります。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>サイトを再インストールする必要があります。どうしたらいいでしょう。

ここに公開されているインストール手順に従 [います](custom_provision.md)。

> [!NOTE]
> 以前のインストールでテレメトリを無効にし、テレメトリを無効にした状態で続行する場合は、ここでテレメトリを無効にする手順に従う必要 [があります](https://github.com/pnp/custom-learning-office-365/blob/a7168c97a76e0b4122e3ddfc530f6a10c724c3e1/installation/README.md)。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>学習経路の実装に関する更新Microsoft 365しました。 サイトを再インストールすると、これらの更新プログラム (サイト テンプレート、再生リスト) が失われるでしょうか。

現在のインストールでサイトを再インストールすると、個々のページとカスタム プレイリストのカスタマイズは失われます。  
