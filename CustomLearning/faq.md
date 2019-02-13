---
author: karuanag
ms.author: karuanag
title: よく寄せられる質問のソリューションを Office 365 のユーザー設定の学習
ms.date: 02/10/2019
description: Office 365 のカスタム学習するための質問の情報を掲載
ms.openlocfilehash: d8b5104e8feeaa4e70296f61594233b27363481b
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952633"
---
# <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. テナント環境に Office 365 のユーザー設定の学習をインストールするための要件とは?

- SharePoint Online との通信のサイトが有効になっています。
- CLO365 を提供している個人は、インストール用のターゲット ・ テナントのテナント管理者である必要があります。
- テナント 'アプリケーション カタログ' は、SharePoint の管理センターの 'アプリケーション' オプションで使用可能なする必要があります。
- CLO365 を提供している個人は、インストールのターゲット ・ テナントのアプリケーション カタログのサイト コレクションの管理者である必要があります。

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. どのような言語は、で利用可能な Office 365 のユーザー設定の学習ですか。

カスタムの Office 365 の学習は、英語のみで現在利用可能です。エンド ・ ツー ・ エンドの自動プロビジョニングは、テナントが英語でのみ機能します。その他の言語は、リリースの将来の追加があります。

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3 テナント環境でサイトをインストールするのには時間がかかりますか。

インストールのテストに基づきと、15 分未満である必要がありますがかかります。これには、お客様の要件にサイトをカスタマイズするために必要な時間は含まれません。

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. 行うものでは、カスタムの Office 365 のプライマリ SharePoint サイト コレクションのサブサイトを学習しますか。

違います。サイトは、ルート サイト コレクションを常に説明したものである、通信のサイト テンプレートに基づきます。

> [!NOTE]
> エンド ・ ユーザーがサイトにアクセスする必要があるアクセス許可を考慮する重要です。ほとんどの組織では、セキュリティまたはユーザーのグループを定義しています。従業員コミュニティにそれを起動する準備ができたら、新しいトレーニング ポータルに適切なセキュリティ グループを追加する必要があります。

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5 サイトを再インストールする必要がある.どうしたらいいでしょう。

インストール手順について公開されている[ここで](installsitepackage.md)次の。

> [!NOTE]
> 「遠隔測定」以前インストール無効にして無効になっている「遠隔測定」を続行したい場合は、指示に従って、ここで「遠隔測定」を無効にするために必要があります。

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. 更新プログラムに加えた Office 365 のユーザー設定の学習の導入。失われます (サイト テンプレートでは、再生リストを作成します)、これらの更新プログラムをサイトを再インストールしている場合ですか。

現在インストールされている上、サイトを再インストールする場合、個々 のページおよびカスタム再生リストのカスタマイズ設定はすべて失われます。  