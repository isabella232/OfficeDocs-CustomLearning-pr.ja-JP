---
author: pkrebs
ms.author: pkrebs
title: 手動インストールのラーニング パス
ms.date: 02/18/2019
manager: bpardi
description: 手動インストールのラーニング パス
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575972"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>ユーザー設定のカスタム 学習を手動でインストールして構成Office 365

Microsoft Custom Learning Web パーツは、バージョン 1.7.1 [SharePoint Frameworkを](/sharepoint/dev/spfx/sharepoint-framework-overview)使用してビルドされます。

Web パーツとサイト コレクションを手動でインストールして構成するには、次の手順を実行する必要があります。

1. すべての前提条件を満たしていることを検証します。
1. テナント アプリ カタログに customlearning.sppkg ファイルOffice 365インストールします。
1. ホーム サイトのカスタム 学習として機能する最新のコミュニケーション サイトをプロビジョニングOffice 365します。
1. カスタム学習が依存する適切な成果物を使用してテナントを構成する PowerShell スクリプトを実行します。
1. CustomLearningAdmin.aspx サイト ページに移動して管理 Web パーツを読み込み、カスタム コンテンツ構成を初期化します。

## <a name="prerequisites"></a>前提条件

テナント全体のアプリ カタログをセットアップして構成している必要があります。 「[アプリ カタログ サイトのOffice 365を設定し、[](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)アプリ カタログ サイトの作成] セクションに従います。 テナント全体のアプリ カタログが既にプロビジョニングされている場合は、このセットアップ プロセスを完了するために、パッケージをアップロードする権限を持つアカウントにアクセスする必要があります。 通常、このアカウントには管理者SharePointがあります。 その役割を持つアカウントが機能しない場合は、SharePoint 管理センターに移動し、アプリ カタログ サイト コレクションのサイト コレクション管理者を見つけて、サイト コレクション管理者の 1 人としてログインするか、サイト コレクション管理者に失敗した SharePoint 管理者アカウントを追加します。 また、テナント管理者の管理者であるアカウントSharePoint必要があります。

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>アップロード Web パーツをテナント アプリ カタログに追加する

カスタム ラーニング を Office 365設定するには、customlearning.sppkg ファイルをテナント全体のアプリ カタログにアップロードして展開します。 アプリ[カタログにアプリを](/sharepoint/use-app-catalog)追加する方法の詳細については、「アプリ カタログを使用して、SharePoint Online 環境でカスタム ビジネス アプリを使用する」を参照してください。

## <a name="provisionidentify-modern-communication-site"></a>モダン コミュニケーション サイトのプロビジョニング/識別

既存の通信サイトをSharePointするか、オンライン テナントに新しい通信サイトをSharePointします。 通信サイトを準備する方法の詳細については[、「SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)で通信サイトを作成する」を参照し、手順に従って通信サイトを作成します。

## <a name="set-permissions-for-the-site"></a>サイトのアクセス許可を設定する

コンテンツを表示できる必要があるすべてのユーザーを Visitors グループに追加し、カスタムプレイリストをメンバー グループに管理できる必要があるすべてのユーザーを追加します。 ユーザーが初めてサイト コレクション管理者または所有者グループの一部である必要がある場合は、カスタム学習用にサイトを構成します。

アプリのカスタム学習Office 365サイト コレクションに追加します。

## <a name="execute-powershell-configuration-script"></a>PowerShell 構成スクリプトの実行

PowerShell スクリプトが含まれているので、ソリューションで使用する 3 つのテナント プロパティを作成するために実行 `CustomLearningConfiguration.ps1` する必要があります。 [](/sharepoint/dev/spfx/tenant-properties) さらに、このスクリプトはサイト ページ[](/sharepoint/dev/spfx/web-parts/single-part-app-pages)ライブラリに 2 つの単一パーツ アプリ ページを作成し、管理者とユーザーの Web パーツを既知の場所でホストします。

### <a name="disabling-telemetry-collection"></a>テレメトリ コレクションの無効化

このソリューションの一部には、匿名化されたテレメトリ追跡オプトインが含まれます。既定ではオンに設定されています。 手動インストールを実行し、テレメトリ追跡をオフにする場合は、スクリプトを変更して、$optInTelemetry 変数を $false `CustomlearningConfiguration.ps1` に設定します。

手動インストールを実行していない場合にテレメトリ追跡をオフにする場合は、実行時にテレメトリ追跡が無効にされる別のスクリプト `TelemetryOptOut.ps1` が含まれています。

## <a name="initialize-web-part-custom-configuration"></a>Web パーツのカスタム構成を初期化する

PowerShell スクリプトが正常に実行された後、に移動します `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。 これにより、初めて使用するカスタム学習を設定する CustomConfig リスト アイテムが初期化されます。

これで構成が完了し、ユーザー設定にカスタム 学習を使用Office 365。 詳細については、ユーザーのドキュメントを参照してください。
