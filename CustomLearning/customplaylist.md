# <a name="customize-the-services-and-playlists"></a><span data-ttu-id="0341e-101">サービスおよび再生リストをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="0341e-101">Customize the Services and Playlists</span></span>

<span data-ttu-id="0341e-p101">既定でサイトの操作性と web パーツの両方に、すべての Office 365 サービスのコンテンツが含まれます。 だけこれらのサービスの全部または一部が、会社で使用可能な場合は、どのようなコンテンツは、ユーザーに利用可能なを調整できます。 この資料では、web パーツのコンテンツをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="0341e-p101">By default both the site experience and the webpart include content for all Office 365 services.  If only all or some of these services are available in your company you can adjust what content is available to your users.  In this article we will customize the webpart content.</span></span>  

## <a name="customizing-the-webpart-content"></a><span data-ttu-id="0341e-105">Web パーツのコンテンツをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="0341e-105">Customizing the webpart content</span></span>

<span data-ttu-id="0341e-106">学習のカスタム web パーツには、2 つの主要機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="0341e-106">The Custom Learning webpart provides two key features:</span></span>
- <span data-ttu-id="0341e-107">テクノロジを表示/非表示</span><span class="sxs-lookup"><span data-stu-id="0341e-107">Hide/Show Technologies</span></span>
- <span data-ttu-id="0341e-108">再生リストを作成します。</span><span class="sxs-lookup"><span data-stu-id="0341e-108">Create a Playlist</span></span>

### <a name="hide-or-show-technology-categories"></a><span data-ttu-id="0341e-109">テクノロジのカテゴリを表示または表示しません。</span><span class="sxs-lookup"><span data-stu-id="0341e-109">Hide or Show Technology Categories</span></span>

<span data-ttu-id="0341e-110">非表示にし、Web パーツにコンテンツを表示します。</span><span class="sxs-lookup"><span data-stu-id="0341e-110">To hide and show content in the Web part:</span></span> 
1.  <span data-ttu-id="0341e-111">、Web パーツのドロップダウン ・ メニューをクリックし、表示/非表示テクノロジをクリックしてください</span><span class="sxs-lookup"><span data-stu-id="0341e-111">Click the dropdown menu on the webpart, then click Hide/Show Technologies</span></span>

![メニュー オプション](media/clohideshow.png)

2. <span data-ttu-id="0341e-113">非表示にする技術および**適用**」を選択するのチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="0341e-113">Select a checkox to hide or show a technology and select **Apply**.</span></span>

![テクノロジー ・ オプション](media/clohideshow1.png)

### <a name="create-a-playlist"></a><span data-ttu-id="0341e-115">再生リストを作成します。</span><span class="sxs-lookup"><span data-stu-id="0341e-115">Create a Playlist</span></span>

<span data-ttu-id="0341e-p102">再生リストは、「資産」の compliation です。「資産」は、SharePoint ページまたはマイクロソフトのトレーニング コンテンツの既存の項目です。一緒に移動する資産を選択した再生リストを作成するとき、ユーザーの学習パスを作成します。</span><span class="sxs-lookup"><span data-stu-id="0341e-p102">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="0341e-p103">SharePoint ページの追加の利点は、YouTube で SharePoint ページを作成することができます、ビデオ、またはビデオを組織でホストされています。フォームやその他の Office 365 のコンテンツにページを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="0341e-p103">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="0341e-121">手順 1: 再生リストの SharePoint ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="0341e-121">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="0341e-p104">この例では、まず、再生リストに追加するのには SharePoint のページを作成します。YouTube のビデオの web パーツと web パーツのテキストを使用してページを作成します。 次の手順では、SharePoint Online のサービスを使用するいると仮定します。</span><span class="sxs-lookup"><span data-stu-id="0341e-p104">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="0341e-125">新しいページを作成します。</span><span class="sxs-lookup"><span data-stu-id="0341e-125">Create a new page</span></span>
1.  <span data-ttu-id="0341e-126">[設定] メニューの [_gt サイト コンテンツ _gt サイト ページ _gt 新しい _gt サイトのページを選択します。</span><span class="sxs-lookup"><span data-stu-id="0341e-126">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="0341e-127">[タイトル] 領域で、[チーム] ボックスを使用する種類</span><span class="sxs-lookup"><span data-stu-id="0341e-127">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="0341e-128">新しいセクションの追加] を選択し、2 つの列を選択します。</span><span class="sxs-lookup"><span data-stu-id="0341e-128">Select the Add a new section, and then select Two Columns.</span></span>

![2 つの列を追加します。](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="0341e-130">左側のボックスで、新しい web パーツの追加を選択し、埋め込みします。</span><span class="sxs-lookup"><span data-stu-id="0341e-130">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="0341e-131">Web ブラウザーでこの URL に移動するhttps://youtu.be/wYrRCRphrp0し、ビデオの埋め込みコードを取得します。</span><span class="sxs-lookup"><span data-stu-id="0341e-131">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="0341e-132">SharePoint の Web パーツでは、コードの埋め込みを追加を選択し、[埋め込み] ボックスに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="0341e-132">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="0341e-133">右側のボックスに、新しい web パーツの追加を選択し、テキストを選択し、します。</span><span class="sxs-lookup"><span data-stu-id="0341e-133">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="0341e-p105">Web ブラウザーでこの URL に移動する: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b 、Try をコピーし、!ページからの指示テキストの Web パーツに貼り付けることとします。ページは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="0341e-p105">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![ページを埋め込む](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="0341e-138">発行] をクリックし、ページの URL をコピーし、メモ帳に貼り付けます</span><span class="sxs-lookup"><span data-stu-id="0341e-138">Click Publish, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="0341e-139">手順 2: 再生リストを作成します。</span><span class="sxs-lookup"><span data-stu-id="0341e-139">Step 2: Create the Playlist</span></span>
1.  <span data-ttu-id="0341e-p106">学習のカスタム web パーツをインストールした場所に移動します。完全なサイトの経験では Office 365 のトレーニングのページでホストされています。</span><span class="sxs-lookup"><span data-stu-id="0341e-p106">Navigate to where you have installed the Custom Learning webpart. In the full site experience it is hosted on the Office 365 training page.</span></span> 
2.  <span data-ttu-id="0341e-142">ドロップダウン ・ メニューから、新しい再生リストの作成を選択します。</span><span class="sxs-lookup"><span data-stu-id="0341e-142">From the dropdown menu select Create New Playlist.</span></span> 

![カスタム再生リストを作成します。](media/clo365createplaylist.png)

3.  <span data-ttu-id="0341e-144">次の例に示すように値を入力し、**作成**を選択します。</span><span class="sxs-lookup"><span data-stu-id="0341e-144">Fill in the values as shown in the example below and select **Create**.</span></span> 

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="0341e-145">手順 3: 再生リストにアセットを追加します。</span><span class="sxs-lookup"><span data-stu-id="0341e-145">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="0341e-146">ここでは、再生リストに、マイクロソフトおよび作成した SharePoint ページから既存の資産を追加します。</span><span class="sxs-lookup"><span data-stu-id="0341e-146">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1.  <span data-ttu-id="0341e-147">メニュー ボタンをクリックし、既存資産の追加] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0341e-147">Click the menu button, then click Add Existing Asset.</span></span>

![資産を追加します。](media/clo365addasset.png)

2.  <span data-ttu-id="0341e-149">Office 365 アプリケーション _gt マイクロソフト チームのトレーニングにフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="0341e-149">Filter on Office 365 Apps > Microsoft Teams Training</span></span>
3.  <span data-ttu-id="0341e-150">マイクロソフトのチームにようこそを追加するチームを取得し、チャットを開始、呼び出しを行います。</span><span class="sxs-lookup"><span data-stu-id="0341e-150">Add Welcome to Microsoft Teams, Get your team up and running, and Start chats and make calls.</span></span>
4.  <span data-ttu-id="0341e-151">メニュー ボタン _gt を作成する資産を選択します。</span><span class="sxs-lookup"><span data-stu-id="0341e-151">Select the menu button > Create Asset.</span></span>
5.  <span data-ttu-id="0341e-152">型では、資産のタイトル] ボックスで [チーム] ボックスを使用します。</span><span class="sxs-lookup"><span data-stu-id="0341e-152">Type Use the Teams command box in the Asset title box.</span></span> 
6.  <span data-ttu-id="0341e-153">SharePoint 使用チーム コマンド ボックス ページのコンテンツ資産] フィールドにコピーした URL を貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="0341e-153">Paste the SharePoint Use the Teams command box page URL you copied in the Asset content field.</span></span> 
7.  <span data-ttu-id="0341e-p107">移動ホーム ページ _gt のカスタム再生リスト _gt に最初のチーム _gt の日が [チーム] ボックスを使用します。ページは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="0341e-p107">Now navigate back to the Home Page > Custom Playlists > Your first days with Teams > Use the Teams command box. Your page should look like the following.</span></span> 

![作成されたページ](media/clo365createplaylist2.png)

<span data-ttu-id="0341e-157">再生リストをこのコンテンツでできるようがインストールされているし、学習のカスタム web パーツが埋め込まれているが任意の場所です。</span><span class="sxs-lookup"><span data-stu-id="0341e-157">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

#### <a name="things-to-think-about"></a><span data-ttu-id="0341e-158">考慮事項</span><span class="sxs-lookup"><span data-stu-id="0341e-158">Things to Think About</span></span>

<span data-ttu-id="0341e-p108">カスタム再生リストは、タスクの vareity で、エンド ・ ユーザーを支援するために使用できます。 要求フォームをオフにしていますか。 ハードウェア機器を要求するためのフォームですか。 作業環境には、既存のトレーニング資料をプログラムできます。</span><span class="sxs-lookup"><span data-stu-id="0341e-p108">Custom playlists can be used to assist your end users in a vareity of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  
