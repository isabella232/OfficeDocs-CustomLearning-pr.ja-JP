---
author: pkrebs
ms.author: pkrebs
title: カスタム学習設定オプション
ms.date: 02/11/2019
description: カスタム学習設定のセットアップオプション
ms.openlocfilehash: d2bb1d98d7eceb63e0cf2bdbf9eead1289641a20
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523011"
---
# <a name="custom-learning-setup-options"></a><span data-ttu-id="6b33d-103">カスタム学習設定オプション</span><span class="sxs-lookup"><span data-stu-id="6b33d-103">Custom Learning Setup Options</span></span>
<span data-ttu-id="6b33d-104">Office 365 のカスタム学習では、ソリューションをさまざまな方法でセットアップできる柔軟性が提供されています。</span><span class="sxs-lookup"><span data-stu-id="6b33d-104">Custom Learning for Office 365 provides the flexibility to set up the solution in a couple different ways.</span></span> <span data-ttu-id="6b33d-105">次のセクションでは、使用可能なオプションの概要を示します。</span><span class="sxs-lookup"><span data-stu-id="6b33d-105">The following sections outline the options available.</span></span>

## <a name="recommended---sharepoint-online-provisioning-service-setup"></a><span data-ttu-id="6b33d-106">推奨-SharePoint Online プロビジョニングサービスのセットアップ</span><span class="sxs-lookup"><span data-stu-id="6b33d-106">Recommended - SharePoint Online Provisioning Service Setup</span></span> 
<span data-ttu-id="6b33d-107">SharePoint Online プロビジョニングサービスは、カスタム学習を設定するための最も高速で簡単な方法として推奨される方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="6b33d-107">The SharePoint Online Provisioning Service provides the fastest, easiest, and recommended method for setting up Custom Learning.</span></span> <span data-ttu-id="6b33d-108">SharePoint Online プロビジョニングサービスでは、Office 365 テナント管理者がサービスにサインインしていくつかの選択を行い、[**テナントに追加**] をクリックしてカスタム学習サイトとカスタム学習 Web パーツをプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="6b33d-108">With the SharePoint Online Provisioning Service, an Office 365 tenant admin signs into the service, makes a few choices, and clicks **Add to Tenant** to provision the Custom Learning Site and the Custom Learning Web part.</span></span> <span data-ttu-id="6b33d-109">プロビジョニングが完了すると、テナント管理者はサイトの準備が整ったことを示す電子メールを受信します。</span><span class="sxs-lookup"><span data-stu-id="6b33d-109">When provisioning is done, the Tenant Admin receives an email that the site is ready to go.</span></span> 

- <span data-ttu-id="6b33d-110">SharePoint のプロビジョニングサービスを開始するには、「 [PnP プロビジョニングサービスを使用してプロビジョニング](custom_provision.md)する」にアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="6b33d-110">To get started with the SharePoint Provisioning Service, go to [Provision with the PnP Provisioning Service](custom_provision.md)</span></span>   

## <a name="stand-alone-custom-learning-web-part-setup"></a><span data-ttu-id="6b33d-111">スタンドアロンカスタム学習 web パーツのセットアップ</span><span class="sxs-lookup"><span data-stu-id="6b33d-111">Stand alone Custom Learning web part setup</span></span>
<span data-ttu-id="6b33d-112">sharepoint online のモダンコミュニケーショントレーニングポータルが既に確立されている組織では、カスタム学習 Web パーツを既存の sharepoint online サイトに手動でインストールするオプションが用意されています。</span><span class="sxs-lookup"><span data-stu-id="6b33d-112">For organizations that already have an established SharePoint Online modern communication training portal, Custom Learning provides the option to manually install the Custom Learning Web part into an existing SharePoint Online site.</span></span> <span data-ttu-id="6b33d-113">サイトは、最新の SharePoint Online サイトである必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6b33d-113">Note that the site must be a modern SharePoint Online site.</span></span> <span data-ttu-id="6b33d-114">このメソッドには、テナント管理者のアクセス許可と、Windows PowerShell または SharePoint Online 管理シェルを使用した環境が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b33d-114">This method requires Tenant Admin permissions and experience with Windows PowerShell or the SharePoint Online Management Shell.</span></span> <span data-ttu-id="6b33d-115">この方法では、SharePoint Online プロビジョニングサービスのセットアップにより多くの技術的な専門知識が必要になることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6b33d-115">Note that this method requires more technical expertise then the SharePoint Online Provisioning Service setup.</span></span>

- <span data-ttu-id="6b33d-116">手動による web パーツのインストール手順については、「 [web パーツを手動でインストールする](custom_manualsetup.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b33d-116">For Manual web part installation instructions, see see [Manually install the web part](custom_manualsetup.md).</span></span> 

## <a name="upgrade-custom-learning"></a><span data-ttu-id="6b33d-117">カスタム学習をアップグレードする</span><span class="sxs-lookup"><span data-stu-id="6b33d-117">Upgrade Custom Learning</span></span>
<span data-ttu-id="6b33d-118">カスタム学習パイロットプログラムに参加しているか、または既にカスタム学習機能がプロビジョニングされている組織では、[カスタム学習の手動アップグレード](custom_upgrade.md)を提供する指示に従うことができます。</span><span class="sxs-lookup"><span data-stu-id="6b33d-118">Organizations that may have participated in a Custom Learning Pilot Program, or already have Custom Learning provisioned, can follow the instruction provided the [Manual Upgrade for Custom Learning](custom_upgrade.md)</span></span>    

### <a name="next-steps---provision-custom-learningcustomprovisionmd"></a><span data-ttu-id="6b33d-119">次のステップ-[カスタム学習のプロビジョニング](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="6b33d-119">Next Steps - [Provision Custom Learning](custom_provision.md)</span></span>
