# 美國中小品牌的 AI 搜尋與 Agentic Commerce 一條龍服務研究

查證日期：2026-10-31，America/Los_Angeles。對象：專案 owner Tony Liu。

**研究結論：值得用付費試點驗證。建議先做「AI 商務通路的導入與代管服務」，從 Shopify 商家的商品資料品質、AI 曝光實測與購買流程開始，再選配物流整合。** 現有平台已提供不少基礎設施，商機在於替缺少人力的品牌把它們設定正確、持續維護，並證明產生什麼價值。

使用者已確認先做美國市場。以下客群範圍、方案、價格與時間均為本研究提出的假設，尚未獲得客戶需求、實際交易或供應商報價驗證。本次完成公開資料研究，沒有取得任何商家後台，也沒有執行真實品牌的曝光、結帳或物流測試。

## 1. 我們賺什麼，商家為什麼付錢

對外的一句話可以是：

> 讓用 AI 找產品的顧客，看得懂你的產品、拿到正確資訊、順利購買；我們替你完成設定、維護與出貨系統串接。

服務包含三層：

| 層次 | 商家的問題 | 我們交付的價值 | 收入方式 |
| --- | --- | --- | --- |
| AI 搜尋與推薦 | 不知道 AI 找不找得到、推薦是否正確 | 基準測試、來源分析、商品頁與資料修復 | 診斷費、導入費 |
| Agent 購物轉換 | 曝光後價格、庫存、運費或付款卡住 | 通路開通、商品資料同步、結帳驗收、異常排查 | 導入費、月費維運 |
| 履約與售後整合 | 系統分散、人工轉單、退貨對帳費時 | 既有 3PL、配送、退換貨系統的設定與協調 | 另計導入費與代管費 |

我們賺專業服務、可重複流程與持續營運的收入。商家與電商平台、支付商、3PL 原則上直接簽約付款；我們不先買庫存、不墊運費、不把物流支出當自己的營收。平台轉介佣金若有，視為可揭露的附加收入，不能支撐主要商業模式。

「只告訴我們三件事」適合做銷售入口。真正上線仍需商家提供帳戶授權、確認商品事實、營業地與銷售地、價格／庫存來源、配送與退款政策。這些可以透過訪談與匯入資料由我們代整理，不能由 AI 憑空補齊。

## 2. 第一批客戶應該是誰

**建議 ICP：已有 Shopify 店、主要向美國消費者銷售、有穩定訂單與清楚差異化，但沒有專職電商技術團隊的品牌。** 商家可以位於美國以外；是否符合各通路資格仍須逐店確認。

初步招募條件是假設：月營收約 US$50,000–300,000、20–300 個可購買變體、owner 或電商主管能核准變更。導入套餐先只涵蓋 100 個變體，額外量另估。營收範圍不是市場統計或平台門檻，用來篩選付費能力與交付複雜度。

優先找家居收納、文具、非電器生活配件等產品：用途與規格容易比較、可用情境明確、適合一般包裹配送。必須先確認平台分類與禁售政策，不能只靠品類名稱判斷。

第一輪不優先接沒有任何銷售基礎的店、只靠低價的無差異商品、B2B 專屬議價、冷鏈、複雜客製、純訂閱或高退貨負擔的品牌。這是降低試點成本的選擇，不代表這些市場沒有需求。例如 Shopify Catalog 本身排除 B2B-only 店面及多種服務／管制類別，開發商店也不能假定有正式通路資格。[Shopify Catalog 資格](https://help.shopify.com/en/manual/shopify-catalog/requirements)

本地服務業與 B2B 是日後另一條路：主要成果會是詢價、預約或合格名單，不能直接套用實體商品 catalog、checkout 與 3PL 的方案。

## 3. 先釐清五種不同成果

| 成果 | 如何證明 | 不能推論成什麼 |
| --- | --- | --- |
| 可抓取 | 頁面回應、robots、CDN 與實際抓取紀錄 | 不等於已收錄 |
| 被發現 | 指定平台的非品牌購物問題出現商品／品牌 | 不等於被推薦或排第一 |
| 被正確推薦 | 使用情境相符、規格與價格正確、有可用商家連結 | 不等於使用者點擊或購買 |
| 能購買 | 指定買家地區、付款與配送條件下完成驗收 | 不等於所有商品／地區可結帳 |
| 帶來商業價值 | 平台訂單、可辨識來源、退款後貢獻與節省工時 | 不等於有因果增量 |

本專案暫用 AEO 命名。業界也使用 GEO、AI visibility、agentic commerce；對商家不用糾結縮寫。報價與驗收必須寫成具體工作與成果。

## 4. AI 與 agent 平台：實際應該優化哪裡

下表為公開官方文件所描述的路徑，**不是本專案已驗證的通路資格**。先確認商家端，再確認買家所在地、帳戶與介面端。平台的公開協議與商家的實際准入分開處理。

| 消費者入口 | 商品／資訊如何進去 | 購買路徑與限制 | 我們該做什麼 |
| --- | --- | --- | --- |
| ChatGPT 搜尋與 Shopping | 網頁搜尋；Shopify Catalog；經核准的直接商品 feed | Shopify 現行文件採導流至商家網站結帳。OpenAI 另有需核准的 Instant Checkout 路徑，不能混用 | 先修 catalog、可抓取頁面與導流結帳；只有確定獲准才規劃直接 ACP checkout |
| OpenAI dots | 官方定位為可使用連接 app、持續承接工作的個人 agent | 沒有從本次文件證實一個獨立、普遍開放的「dot 商品排名／送件」機制 | 當作可發現與可操作性的驗收入口；不要另外出售未證實的 dot 排名服務 |
| Google AI Overviews／AI Mode | Google Search 索引；購物資料另有 Merchant Center | 一般引用與 shopping checkout 是不同能力；UCP checkout 限參與商家／合作夥伴並逐步開放 | 同步做基本 SEO、Merchant Center 資料修復與可用 checkout 驗收 |
| Gemini | 商品發現可利用 Google 購物生態；直接購買有 UCP 整合路徑 | Google 文件涵蓋美國、加拿大、澳洲的合資格產品／參與者；不同介面 rollout 不同 | 美國優先，實測所用帳戶與介面；不可把 UCP 實作等同獲准上架 |
| Microsoft Copilot | Shopify Catalog／商家整合計畫 | Shopify 合資格、銷售至美國的商家可用 direct checkout；非 Shopify 有申請路徑 | 加入試點主力；測搜尋、價格、稅運費、付款與訂單來源 |
| Meta AI／Muse | Shopify Catalog；部分表面還需要 Facebook & Instagram 通路資料同步 | Shopify 提供有條件的 Meta direct checkout，Muse 視可用性；不同地區／介面不能相互推定 | 測資料同步與可用介面，核對限制與 fallback，依實際可用性納入 |
| Claude | 網頁搜尋／使用者抓取；commerce blueprint、連接器或商家自建購物 agent | 有公開商務建構工具，不等於有一個所有 SMB 都可投稿的統一購物 marketplace／直接結帳入口 | 檢查搜尋抓取、來源引用；有客戶需求再建 connector 或站內購物助手 |
| Apple Siri／Apple Intelligence | Applebot 相關搜尋；部分問題可使用 ChatGPT | 本次未證實普遍可申請的獨立 Apple agent 商品 feed／商家 checkout 入口；Apple Pay 本身不代表商品被推薦 | 維持公開資訊與 Applebot 可讀性，測具體 Siri 問題與導流，不先賣 Apple 專屬開通 |
| Perplexity | 商家商品整合、網頁搜尋與合作平台 | 官方描述 PayPal 驅動的 Instant Buy，商家保留交易主體角色；不可假定每個地區、商家皆可用 | 視 Feedonomics／支付商等既有路徑評估准入，再測購買與售後 |

依據：[OpenAI feed 准入](https://developers.openai.com/commerce/guides/get-started)、[OpenAI checkout](https://developers.openai.com/commerce/specs/checkout)、[dots 官方說明](https://learn.chatgpt.com/docs/enterprise/dots-admin-guide)、[Shopify ChatGPT](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/chatgpt)、[Google AI features](https://developers.google.com/search/docs/appearance/ai-features)、[Google UCP 資格](https://support.google.com/merchants/answer/16837055?hl=en)、[Copilot](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/microsoft)、[Meta/Muse](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/meta)、[Claude commerce](https://platform.claude.com/docs/en/about-claude/use-case-guides/commerce-agents)、[Apple Siri](https://support.apple.com/guide/iphone/use-siri-to-get-answers-from-chatgpt-iph0193a9d54/27/ios/27)、[Applebot](https://support.apple.com/en-us/119829)、[Perplexity](https://www.perplexity.ai/en-GB/hub/blog/shopping-that-puts-you-first)。

你提到的「.dot」可對應已查證的 dots，「Meta Muse」也有官方文件；「Cloud 的 Do It」暫無法確認正式名稱。此報告先涵蓋 Claude 搜尋與 commerce 能力，不把 Do It 擅自改名為 Cowork。

### Shopify checkout 的關鍵差異

不能拿早期公告寫成「所有 Shopify 商品都能在 ChatGPT 內直接結帳」。截至本次查證，Shopify 的 ChatGPT 通路說明明確表示是商品發現與導流，後台沒有 ChatGPT direct checkout 開關；而 OpenAI 的一般 checkout 規格仍描述核准合作夥伴的整合。兩份文件講的是不同路徑，專案估價以客戶實際路徑為準。[Shopify 說明](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/chatgpt)、[OpenAI 規格](https://developers.openai.com/commerce/specs/checkout)

Google 的 Shopify 路徑需要有效 Merchant Center 與商品資料，direct checkout 仍逐步 rollout；美國在文件資格範圍內，不代表客戶帳戶已收到功能。[Shopify Google 通路](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/google)

Meta 路徑需留意：direct checkout 不支援部分商品類型與配送方式，含 bundle、純訂閱、客製、B2B-only 及取貨點等；客戶端 GA／custom pixels 不會像一般網店結帳一樣觸發。因此我們要用平台訂單與伺服器事件核對，不能只看 GA4。[Meta 功能限制與訂單歸因](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/meta)

## 5. Shopify 以外，有哪些路徑

| 選項 | 已查到的官方能力 | 適用情況與交付成本判斷 |
| --- | --- | --- |
| Shopify 原生商店 | Catalog、agentic storefronts、knowledge base 與通路管理 | 第一個交付範本；仍需資料修復、資格檢查與維護 |
| Shopify Agentic plan | 可保留外部網店；不同通路有 discovery 或 Shopify-powered checkout 設定 | 不必一開始要求客戶搬站；需評估商品／庫存／訂單雙系統同步成本 |
| WooCommerce | WooCommerce AI 有 UCP 開關與 discovery document；仍需外部購物服務 onboarding 和支援付款方式 | 適合已有 WordPress 團隊的客戶；插件版本、相容性與維護成本較高 |
| BigCommerce + Feedonomics | 商品資料 enrichment 與對外分發，部分能力區分 available／early access | 適合目錄複雜與多通路商家；各通路必須個別確認，取得報價後再算毛利 |
| Wix | 官方描述商品分發、協議整合與站內 agent 能力，部分分批開放 | 已在 Wix 的小品牌先保留平台，從後台可用性與 feed 入手 |
| Shopware + PayPal | PayPal Agentic Commerce sales channel，要求合資格商業帳戶及 extension | 後續有既有 Shopware 客戶再做；不作美國初期標準套餐 |
| 既有／自建網店 + Stripe Agentic Commerce Suite | 分享 catalog，由 Stripe 管理 checkout、支付及訂單通知；也有自訂／自管路徑 | 可作第二種標準整合，先查可用國家、平台和 hooks 限制 |
| SHOPLINE 等在地平台 | 可先用公開網頁與既有商品 feed；目前查到的站內 AI assistant 不足以證明外部 agent 直接結帳 | 美國第一階段暫不投入專屬 adapter；有付費客戶才做逐項查證 |

來源：[Shopify Agentic plan](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/agentic-plan-setup)、[WooCommerce UCP](https://woocommerce.com/document/woocommerce-ai/agentic-commerce/)、[BigCommerce](https://www.bigcommerce.com/product/agentic-commerce/)、[Feedonomics](https://feedonomics.com/product/agentic-commerce/)、[Wix](https://www.wix.com/studio/ai-search-lab/agentic-commerce)、[Shopware](https://docs.shopware.com/en/shopware-6-en/extensions/paypal)、[Stripe 零售路徑](https://docs.stripe.com/agentic-commerce/sellers/use-cases/retail.md)、[SHOPLINE 功能狀態](https://support.shoplineapp.com/hc/en-us/articles/62243748056601--Coming-Soon-AI-Shopping-Assistant-Message-Center)。

**選平台的原則：先改善客戶既有環境。** 搬站只有在原平台確實阻擋關鍵商務需求，而且收入／營運效益足以負擔遷移成本時才提案。支付商可處理交易，不會自動替品牌建立可信內容；feed 工具可送資料，也不代表已取得每個 agent 的准入。

### 不同協議各做什麼

- Schema.org／JSON-LD：頁面的機器可讀事實，與可見內容一致。
- Product feed／Catalog：持續交換商品、價格、庫存、圖片與購買連結。
- ACP：OpenAI 商務整合規格；feed 與 checkout 的資格分開。
- UCP：商務互動與 checkout 能力協議；Google 提供採用路徑與准入流程。
- MCP：讓 agent 呼叫工具的介面；自己建 MCP server 不代表消費者 agent 會發現或使用它。
- 支付憑證／wallet：解決授權與支付傳遞，不是搜尋排名機制。

技術依據：[OpenAI commerce](https://developers.openai.com/commerce)、[Google UCP](https://developers.google.com/merchant/ucp)、[Stripe 商務概念](https://docs.stripe.com/agentic-commerce)。初期優先平台代管，避免每家 SMB 都從零建一套協議端點。

## 6. 我們具體怎麼優化 agent 搜尋

### A. 先建立可重複的搜尋基準

每家先選 30 個具有購買意圖的問題，固定美國／英文與測試時點：10 個產品用途、10 個條件比較、5 個預算／配送、5 個品牌準確性問題。品牌問題與非品牌問題分開看，避免以容易成功的品牌查詢美化成效。

例如家居品牌：「Best under-sink organizer for a narrow cabinet under $50」「Which organizer fits a 12-inch cabinet and ships to California?」。只有產品確實符合尺寸與配送條件才算推薦正確。

首輪 ChatGPT、Google 的指定 AI 搜尋介面、Copilot 各重跑 3 次，共 270 次觀測。保存回答、引用 URL、商品卡、連到哪個 seller、價格與可購買狀態。Google 未觸發 AI 回答也記錄，不能只挑出現時取樣。Claude、Muse、Siri、Perplexity 做少量探索，待准入與客戶需求明確再擴大。

API 的回答與消費者 app 的 shopping UI 分開標記；不以 API 模型測試代替實際商品卡驗證。執行方式先使用人工抽樣、官方允許介面或已有合適權限的服務；先確認成本與可用性。

### B. 修復可讀與可索引性

檢查 robots.txt、noindex、canonical、sitemap、頁面狀態碼、內部連結、手機呈現與 CDN/WAF；確保商品主要內容不只存在難以取得的互動層。記錄真實抓取結果；模擬 User-Agent 的 200 回應只是基本檢查，不能證明平台真的收錄。

OpenAI 的 OAI-SearchBot 與訓練用 GPTBot 可分開設定；Claude 也分 Claude-SearchBot、Claude-User 與 ClaudeBot。商家不必為追求搜尋曝光就無差別開放訓練爬蟲。Applebot 與 Applebot-Extended 也有不同用途。[OpenAI bots](https://developers.openai.com/api/docs/bots)、[Anthropic bots](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler)、[Applebot](https://support.apple.com/en-us/119829)

Google 明確表示 AI Overviews／AI Mode 延用 SEO 基礎，沒有特殊必要的 AI 檔案或 schema；因此 `llms.txt` 可列低成本選配，不應當成主要交付或保證排名的手段。[Google 官方指引](https://developers.google.com/search/docs/appearance/ai-features)

### C. 把商品變成可準確比較的資料

內部建立每個可購買變體的統一紀錄：穩定 ID、SKU、品牌、真實 GTIN／MPN（有才填）、尺寸／材質／容量／相容性、用途、限制、圖片、價格／幣別、庫存、URL、配送地與時效、退貨政策、資料來源與更新時間。

每個欄位要標明權威系統：商品內容由商家／PIM 確認；價格由 commerce 系統；庫存由店家或 WMS；出貨時效由實際履約設定。缺資料標記待補，不生成不存在的認證、評價或規格。

Shopify 的 product category 是標準分類；category metafields 是分類對應屬性；collections 是商店的陳列分組。Google 分類又是另一個 mapping。不能只建立 collections 就聲稱完成 taxonomy。官方說明 category metafields 能補充有助商品發現的屬性，但不是排名保證。[Shopify category metafields](https://help.shopify.com/en/manual/custom-data/metafields/category-metafields)

### D. 同步頁面、結構化資料與 feed

商品頁回答「適合誰、哪種情境、規格、和替代方案差在哪、限制、何時收到、怎麼退」。寫能核實的比較與 FAQ，補品牌身份、聯絡方式、保固與真實使用證據。選擇具購買意圖的內容，不靠批量空泛文章。

在適用頁面核對 Product、Offer、變體、配送／退貨等結構化資訊；價格、庫存與可見頁面一致。用 Rich Results Test、Search Console 與 Merchant Center 診斷確認；語法正確與被展示分開。Google 建議商品資料放在 initial HTML，並提醒動態產生資料可能影響快速變動資訊的可靠性。[Google merchant listing 規格](https://developers.google.com/search/docs/appearance/structured-data/merchant-listing)

先用 Shopify／Google 原生連接器；有大量渠道才評估 Feedonomics。若走 OpenAI 直接 feed，依當時 Stable schema 與帳戶核准路徑映射，feed 准入和 checkout 是不同設定。不要用一份自創 CSV 宣稱已上架所有 agent。[OpenAI product schema](https://developers.openai.com/commerce/specs/file-upload/products)

品牌站以外，整理真實通路商品頁、零售商資料、可信評測與社群內容中的品牌／規格一致性。此為提升可驗證資訊供給的策略推論，不是各平台公開的排名公式，也不承諾付費發文能換到推薦。

### E. 從曝光一路驗證到訂單

修復後重跑原查詢組，比較推薦率、引用率、商品卡、資訊準確率與 seller 連結。另測落地頁、變體、加車、運費、折扣、付款、訂單通知與出貨狀態。若 direct checkout 不支援，就把回商店完成購買的路徑做好。

## 7. 物流與退換貨：如何提供一條龍

買家 agent → 商家 commerce／OMS → 3PL 或既有倉庫 → 承運商 → 追蹤通知 → 退貨 portal → 倉庫驗收 → 商家退款／換貨。**訂單以商家 commerce 系統為中心**；物流不應為每一種 AI 入口各自建一份。

| 需求層 | 可評估服務 | 提供什麼 | 我們負責什麼 |
| --- | --- | --- | --- |
| 委外倉儲、揀貨、包裝 | Flexport、ShipBob | 實體履約；商品與服務資格、庫存及地區另確認 | 比對報價、SKU 對應、入倉與路由設定、測試訂單 |
| 商家已有倉庫，需要寄件系統 | ShipStation、Shippo | 訂單匯入、運價／標籤、追蹤或 API | 配送規則、欄位同步、失敗重送與追蹤回寫 |
| 跨境配送工具 | Easyship | Shopify 訂單同步、部分 checkout 即時運價與稅費呈現能力 | 核對方案限制、寄件地、運輸服務與實際費用；不可只靠展示估價承諾全額到岸成本 |
| 退換貨流程管理 | Shopify 原生流程；成長後選 Loop 或 AfterShip Returns | 退貨申請、規則、標籤、換貨、狀態與 3PL 串接 | 設定政策、倉庫收貨與退款觸發、驗證庫存與金額 |

官方依據：[Flexport 與 Shopify](https://help.shopify.com/en/manual/fulfillment/shopify-fulfillment-network/logistics-partners/flexport-getting-started)、[ShipBob Shopify](https://partners.shipbob.com/directory/shopify)、[ShipBob Returns API](https://developer.shipbob.com/guides/returns)、[ShipStation](https://www.shipstation.com/partners/shopify/)、[Shippo](https://goshippo.com/products/api)、[Easyship Shopify](https://support.easyship.com/hc/en-us/articles/19224078074258-Connect-Your-Shopify-Store)、[Loop](https://www.loopreturns.com/faq/)、[AfterShip](https://www.aftership.com/returns)。

**初期不要預設幫商家換 3PL。** 已有可靠倉庫就保留，先把 AI 來源訂單接回同一套流程。只有現有履約無法滿足時效、庫存同步或退貨需求時才提替換。選 3PL 需比較收貨、倉租、首件／加件、包材、配送分區／材積、退貨檢驗、銷毀、月最低費、旺季附加與退場移倉成本。ShipBob 官方採客製報價，不能套網路上的單一每單價格。[ShipBob 報價資訊](https://www.shipbob.com/pricing/)

逆物流要分清：建立退貨申請 ≠ 包裹已收到；收到 ≠ 檢驗可再銷售；檢驗通過 ≠ 已退款。只允許一個系統負責回補可售庫存、一個系統負責退款。Loop 的 Shopify native exchange 會連回原訂單，整合時要查使用中的流程，避免沿用舊的另開換貨單假設。[Loop native exchange](https://help.loopreturns.com/en/articles/2771905)

對商家，我們提供一個窗口、共用工單與供應商協調。倉庫實際收貨、承運商配送、商家退款核准仍依各方責任執行；我們以處理和追蹤異常收費。代管時段、超量工單與緊急聯繫要寫清楚，side project 初期不能承諾全天候人工支援。

## 8. 商業模式與單位經濟

以下是**待試賣的美元報價假設**，不是市場行情或供應商報價：

| 方案 | 假設售價 | 範圍 | 要驗證的事情 |
| --- | --- | --- | --- |
| 付費診斷 | US$500／次 | 1 個店、抽樣商品、搜尋樣本、資格與修復清單 | owner 是否願意為具體修復機會付錢 |
| 標準導入 | US$3,500／次 | 1 店／美國英文／最多 100 變體；選定通路與一套結帳流程；不含搬站或換倉 | 能否在約 24 小時直接工時完成 |
| 月費維運 | US$1,200／月 | 約 6 小時服務工時、資料健康檢查、固定搜尋樣本、月報與限量修復 | 是否有持續問題和續約價值 |
| 物流整合加值 | 另案估價 | 保留既有或導入一個 3PL、一個退貨流程；另訂工單額度 | 不同商家差異是否可標準化 |

第三方軟體、支付、物流與稅費另付；若診斷費折抵導入費，試算收入也要扣除，不得重複計算。

以 owner 時間 US$75／小時的內部成本假設計算：

- 診斷：500 − 4 小時 × 75 − 50 工具成本 = **150（30%）**。
- 導入：3,500 − 24 小時 × 75 − 200 工具／直接支出 = **1,500（約 43%）**。
- 維運：1,200 − 6 小時 × 75 − 150 分攤工具成本 = **600（50%）**。

以上是扣直接服務成本後的貢獻，尚未扣獲客、行政、稅、設備與沒有收費的維護。若維運花到 12 小時，貢獻降為 150；若工具每客戶是 400，6 小時服務的貢獻只剩 350。定價是否成立，很大程度取決於範圍管理與工時。

對商家也要算帳：假設每筆新增完成訂單客單 US$80，扣商品、支付、配送補貼及預期退貨等變動成本後剩 US$24，US$1,200 月費要約 **50 筆真正新增訂單**才打平。若把 3,500 導入費攤 6 個月，每月總負擔約 1,783，需 **75 筆**。這是敏感度例子，不能拿 50 筆平台歸因訂單直接當新增訂單。

若客戶無法合理期待足夠新增貢獻或可證明的人力節省，只出售一次診斷與修復。物流節省要用實際帳單及工時證明，不能和新增訂單重複計算。

Side project 的初期容量也有限：5 家維運約 30 小時／月，再加 1 家導入 24 小時、銷售與行政 15 小時，共約 **69 小時／月**。假設收入 5 × 1,200 + 3,500 = 9,500，其中經常性月收入是 6,000；以同樣假設扣服務成本後約 4,500，再扣銷售行政時間 1,125，剩約 3,375，尚未扣其他費用。這是情境，不是收入預測。先驗證 owner 可投入時間，再設接案上限。

## 9. 競爭、差異化與風險

已存在三種直接替代品：

| 類型 | 已有代表與能力 | 我們必須多提供什麼 |
| --- | --- | --- |
| 平台內建 | Shopify agentic storefronts；Wix 與 WooCommerce 等原生能力 | 跨設定問題排查、商家資料清理、實際驗收與維運 |
| AI 搜尋觀測 | Peec AI；Profound Shopping 可觀測商品卡、商家連結與價格 | 從報表走到修改、上線與訂單／履約結果，不只交 dashboard |
| Feed 管理與分發 | Feedonomics 等商品資料平台 | 幫 SMB 選擇必要工具、維護來源真實性與通路資格，並控制總成本 |

依據：[Shopify](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts)、[Peec AI](https://peec.ai/)、[Profound Shopping](https://help.tryprofound.com/articles/8862399588-about-shopping)、[Feedonomics](https://feedonomics.com/product/agentic-commerce/)。這些是供應商自述功能，不代表本專案已評測它們的資料品質或投資報酬。

我們可累積的優勢是：同一垂直品類的查詢與商品屬性知識、可重複的修復流程、變更與結果紀錄、異常排查能力及供應商協調。初期這些只是要建立的能力，不能當成已擁有的護城河。

主要風險與對策：平台自行把設定簡化 → 服務重心放在營運；曝光少或不穩定 → 小樣本重跑並延長觀察；來源歸因不完整 → 平台訂單＋網站流量＋定期訪談分開看；客製服務爆量 → 限定平台／SKU／時數；物流掩蓋 AEO 效益 → 物流另案衡量；更新推翻原判斷 → 每月重查通路資格與功能，保留查證日期。

## 10. Owner 現在應採取的路線

建議用 90 天回答三件事：有人願意付錢嗎、能在限定工時交付嗎、有足夠價值支持續約嗎。先做 10 次訪談，找 3 家有真實訂單的付費試點；從 1 家的 100 個以內變體與 2–3 個通路做完整交付。物流先整合既有流程，等客戶願意付費再擴充換倉與更複雜退換貨。

第一個可賣成果應是一份「具證據的診斷＋已修復的商品資料＋可購買的通路＋可追蹤的結果」。等三家試點證明共同需求，再把匯入、欄位驗證、feed 健康與報表自動化。不要在付費需求尚未成立前先造大型 agent 平台。

詳細執行見 [服務 pipeline](../service-pipeline.md)、[90 天計畫](../roadmap.md) 與 [查證紀錄](sources.md)。
