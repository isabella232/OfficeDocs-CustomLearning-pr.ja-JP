---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 学習経路のトラブルシューティング
ms.date: 02/10/2019
description: Microsoft 365 ラーニング パスのトラブルシューティング方法について説明します。
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000303"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Microsoft 365 ラーニング パスのトラブルシューティング

Microsoft 365 ラーニング パスまたは SharePoint Online プロビジョニング サービスで発生する可能性がある問題のトラブルシューティングのヒントを次に示します。

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>テナント管理者のアクセス許可を持っているかどうかの確認方法

SharePoint Online Provisioning Service にサインインし、カスタム 学習をプロビジョニングするには、テナント管理者のアクセス許可が必要です。 SharePoint Online Provisioning Service でサインインに関する問題が発生している場合は、グローバル管理者の役割が割り当てられていることを確認してください。 カスタム 学習ソリューションには、テナント管理者のアクセス許可 (365 グローバル管理者Officeと呼ばれる) が必要です。 グローバル管理者の役割が割り当てられているかどうかを確認する方法を次に示します。

1.  サインインして Office.com。
2.  [管理者 **] をクリックします。**
3.  [ユーザー **] で**、[アクティブな **ユーザー] を選択します。**
4.  名前を検索する
5.  [検索結果] で自分の名前をクリックします。 役割のグローバル管理者が表示されます。
![ライセンス、グループ メンバーシップ、その他の情報と共に役割を一覧表示するサンプル ページ。](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>グローバル管理者の役割を持ってない場合
- 組織でグローバル管理者を見つけて、そのユーザーにサービスにサインインするか、グローバル管理者の役割を割り当てします。

## <a name="tenant-app-catalog-troubleshooting"></a>テナント アプリ カタログのトラブルシューティング
カスタム学習では、ターゲット テナントにアプリ カタログをプロビジョニングする必要があります。 アプリ カタログを作成するには、グローバル管理者のアクセス許可が必要です。 アプリ カタログに関する一般的な問題のトラブルシューティング手順を次に示します。

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>テナント アプリ カタログを持っているかどうかの確認方法 
まず、グローバル管理者のアクセス許可を持っている必要があります。 上記の「テナント管理者のアクセス許可」の手順を参照してください。

1. [Office 365 から、[**管理**] をクリックし、[展開] 矢印をクリック>、[すべての管理センター SharePoint を表示する]  >    >  **をクリックします**。
2. [**従来の管理 SharePoint Center アプリ**  >  **アプリ**  >  **カタログ] をクリックします**。
3. [ **アプリ] の** 下に、[SharePoint 用アプリの配布 **] というタイトルのタイルが表示されます**。 タイルが表示される場合は、テナント アプリ カタログがあります。 以下の **「サイト の Colllection...」** セクションを参照してください。 タイルが表示されていない場合は、テナント用のテナント アプリ カタログを作成する必要があります。 以下の「 **テナント アプリ カタログを作成する方法」** セクションを参照してください。

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>テナント アプリ カタログのサイト コレクション所有者を確認する方法 
Microsoft 365 ラーニング パスをプロビジョニングするには、テナント アプリ カタログのサイト コレクション所有者である必要があります。 所有者かどうかを確認する方法を次に示します。

1. [Office 365 から、[**管理**] をクリックし、[展開] 矢印をクリック>、[すべての管理センター SharePoint を表示する]  >    >  **をクリックします**。
2. [ **クラシック管理 SharePoint センター] をクリック** し、アプリ カタログ **を選択します**。
3. [ **所有者] を** 選択し、サイト コレクションの所有者を確認します。 これは次のように見える必要があります。
![[管理者の管理] ページ。](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>テナント アプリ カタログが存在しない場合の作成方法 
1. SharePoint Online 管理者Office 365 にサインインします。
2. **[管理者]** をクリックします。
3. [管理 **センター] で****、[SharePoint] をクリックします**。 
4. [アプリ **アプリ**  >  **カタログ] をクリックします**。
5. [新 **しいアプリ カタログ サイトの作成] をクリック** し **、[OK] をクリックします**。 
6.  アプリ カタログの情報を入力します。 複数の管理者を含める場合があります。 次に例を示します。  
![新しいアプリ カタログの情報を入力するフォーム。](media/cg-appcatalogfinish.png)

7.  これで完了です。 完了です。 ただし、カスタム 学習のプロビジョニングに移行する前に、アプリ カタログの作成が完了するまで少なくとも 30 分待つ必要があります。 

> [!IMPORTANT]
> カスタム学習をプロビジョニングする前に、テナント アプリ カタログを作成してから少なくとも 30 分待ちます。 これにより、SharePoint 内でアプリ カタログのプロビジョニング プロセスが完了します。 