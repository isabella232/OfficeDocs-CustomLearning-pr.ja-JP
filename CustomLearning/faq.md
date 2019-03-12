---
author: karuanag
ms.author: karuanag
title: Office 365 ソリューションのカスタム学習に関してよく寄せられる質問
ms.date: 02/10/2019
description: Office 365 のカスタム学習に関するよく寄せられる質問の情報
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: c60ca83b784f36b6f41b56ac193f7d58c750984e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/12/2019
ms.locfileid: "30543767"
---
# <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. Office 365 用のカスタム学習をテナント環境にインストールするための要件は何ですか。

- SharePoint Online とコミュニケーションサイトが有効になっている。
- CLO365 をプロビジョニングするユーザーは、インストール先のテナントのテナント管理者である必要があります。
- テナント ' App Catalog ' は、SharePoint 管理センターの [アプリ] オプション内で使用できる必要があります。
- CLO365 をプロビジョニングするユーザーは、インストール先のテナントのアプリカタログのサイトコレクション管理者である必要があります。

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. どの言語が Office 365 用のカスタム学習で利用できますか?

Office 365 のカスタム学習は、現在英語版でのみ利用可能です。 自動エンドツーエンドプロビジョニングは、英語のテナントでのみ機能します。 今後のリリースでは、追加の言語が追加される場合があります。

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. テナント環境にサイトをインストールするのにどれくらいの時間がかかりますか?

インストールのテストに基づき、15分未満で完了する必要があります。 これには、要件に合わせてサイトをカスタマイズするのに必要な時間は含まれません。

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. Office 365 のカスタム学習は、プライマリ SharePoint サイトコレクションのサブサイトにすることができますか。

いいえ。 サイトは、コミュニケーションサイトテンプレートに基づいています。これは、常にルートサイトコレクションであることを意図しています。

> [!NOTE]
> エンドユーザーがサイトにアクセスするために必要なアクセス許可について考慮することが重要です。 多くの組織では、セキュリティまたはユーザーグループを定義しています。 従業員コミュニティに対してを開始する準備ができたら、適切なセキュリティグループを新しいトレーニングポータルに追加する必要があります。

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. サイトを再インストールする必要があります。どうしたらいいでしょう。

[ここで](custom_provision.md)公開されているインストール手順に従います。

> [!NOTE]
> 以前のインストールでテレメトリを無効にしていて、テレメトリを無効にしたままにする場合は、ここでテレメトリを無効にするための手順に従う必要があります。

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. Office 365 のカスタム学習の実装を更新しました。 サイトを再インストールすると、これらの更新プログラム (サイトテンプレート、再生リストに加えられたもの) は失われますか?

現在のインストール環境でサイトを再インストールすると、個々のページおよびカスタム再生リストに対するカスタマイズが失われます。  