# 官方來源與查證紀錄

查證日期：2026-10-31（America/Los_Angeles）。來源採公開官方產品、Help Center、開發文件與供應商文件；不以社群推測當成平台能力。本紀錄是查閱時的摘要，連結內容可能持續更新；未保存整份網頁快照。沒有商家後台、正式准入或真實交易驗證。

## 證據如何使用

- 「官方文件描述」：能支持功能或流程存在，不代表個別商家能用。
- 「受限／rollout」：有資格、審核、地區、帳戶或介面限制，須逐店查驗。
- 「供應商自述」：可作候選工具清單，不當作獨立實測、效益或排名證據。
- 「未證實」：本次資料不足，不能寫成不存在，也不能對客戶承諾。

所有研究建議、報價、工時、客群門檻、試點數與成效目標都是專案假設，未從下列文件推導成市場統計。

## AI／agent 與商務協議

| ID | 官方來源 | 支持的判斷／限制 |
| --- | --- | --- |
| A01 | [OpenAI — Get Started](https://developers.openai.com/commerce/guides/get-started) | 直接商品 feed onboarding 對核准合作夥伴開放；實作前查准入 |
| A02 | [OpenAI — Products file upload schema](https://developers.openai.com/commerce/specs/file-upload/products) | Stable／Draft 區分、變體與資料欄位；checkout 需另外啟用，旗標不等於完成准入 |
| A03 | [OpenAI — Agentic Checkout Spec](https://developers.openai.com/commerce/specs/checkout) | 公開 checkout 整合規格；Instant Checkout 對核准合作夥伴開放 |
| A04 | [OpenAI — Commerce](https://developers.openai.com/commerce) | ACP 的商品與商務整合定位 |
| A05 | [OpenAI — Crawlers](https://developers.openai.com/api/docs/bots) | OAI-SearchBot、GPTBot 與使用者導向抓取的區別；不可把訓練與搜尋開放綁在一起 |
| A06 | [ChatGPT Learn — Dots admin guide](https://learn.chatgpt.com/docs/enterprise/dots-admin-guide) | dots 的持續工作、app 與執行權限；沒有據此證實獨立商家排名／feed 系統 |
| A07 | [Google — AI features and your website](https://developers.google.com/search/docs/appearance/ai-features) | 延用 SEO 基礎，不需特殊 AI 檔案或 schema；Search Console 的 AI 搜尋資料不宜假定可完整獨立拆出 |
| A08 | [Google — Merchant listing structured data](https://developers.google.com/search/docs/appearance/structured-data/merchant-listing) | 商品、Offer、變體與政策資料；initial HTML 建議；標記不保證展示 |
| A09 | [Google — UCP guide](https://developers.google.com/merchant/ucp) | Merchant Center、UCP、native／embedded checkout 與 waitlist；介面可用性仍須確認 |
| A10 | [Google Merchant Center — UCP eligibility](https://support.google.com/merchants/answer/16837055?hl=en) | 美國、加拿大、澳洲的合資格產品與參與商家／夥伴；rollout 不等於全體可用 |
| A11 | [Claude — Commerce agent](https://platform.claude.com/docs/en/about-claude/use-case-guides/commerce-agents) | 購物與商家 agent 的公開 blueprint；不能推成消費者統一購物目錄 |
| A12 | [Anthropic — Crawler controls](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) | ClaudeBot、Claude-User、Claude-SearchBot 的不同作用 |
| A13 | [Apple — Siri using ChatGPT](https://support.apple.com/guide/iphone/use-siri-to-get-answers-from-chatgpt-iph0193a9d54/27/ios/27) | Apple Intelligence／Siri 的 ChatGPT 路徑；不能推成獨立 Apple 商務 feed |
| A14 | [Apple — About Applebot](https://support.apple.com/en-us/119829) | Applebot 的搜尋用途與 Applebot-Extended 控制；不是購物排序公式 |
| A15 | [Meta — Introducing Muse](https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/) | 證實 Muse 個人 agent；與模型 Muse Spark 或一般 Meta AI 介面分開描述 |
| A16 | [Microsoft — Copilot Checkout and Brand Agents](https://about.ads.microsoft.com/en/blog/post/january-2026/conversations-that-convert-copilot-checkout-and-brand-agents) | Shopify 與非 Shopify 的合作／申請路徑；早期公告不能代替現行商家資格 |
| A17 | [Perplexity — Shopping That Puts You First](https://www.perplexity.ai/en-GB/hub/blog/shopping-that-puts-you-first) | 描述 PayPal Instant Buy 與商家角色；此網址區域前綴不是購物功能地域資格的證據 |

## Shopify 的實際通路文件

| ID | 官方來源 | 支持的判斷／限制 |
| --- | --- | --- |
| S01 | [Agentic storefronts](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts) | Catalog／其他通路、knowledge base、直接購買與導流的不同路徑 |
| S02 | [Selling on ChatGPT](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/chatgpt) | 現行 Shopify 路徑為 discovery／商家網店 checkout；銷售至美國；不存在此通路的 direct checkout 開關 |
| S03 | [Selling on Google AI Mode and Gemini](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/google) | Google Merchant Center、商品同步、direct checkout rollout 與地區條件 |
| S04 | [Selling on Microsoft Copilot](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/microsoft) | 美國銷售與 Shopify Catalog 等資格；direct checkout 與 opt-out 路徑 |
| S05 | [Selling on Meta](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/meta) | Meta direct checkout、Muse 可用性、國家、商品與配送限制、pixels 與訂單歸因 |
| S06 | [Shopify Catalog requirements](https://help.shopify.com/en/manual/shopify-catalog/requirements) | 方案、公開商品、帳戶信譽／營運歷史、開發商店與禁用類別等資格 |
| S07 | [Agentic plan setup](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/agentic-plan-setup) | 保留既有非 Shopify 網店的路徑；direct checkout 預設關閉，按通路設置 |
| S08 | [Catalog and product discovery](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/products) | 不同通路使用 Catalog／Google／Meta 資料路徑，不可假定共用單一 feed |
| S09 | [Category metafields](https://help.shopify.com/en/manual/custom-data/metafields/category-metafields) | 標準分類對應商品屬性，有助資料完整性與商品發現 |
| S10 | [Knowledge base](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts/knowledge-base) | 非商品資訊與商家政策的維護入口；實作時重查帳戶可用功能 |

## 其他平台與替代服務

| ID | 官方來源 | 支持的判斷／限制 |
| --- | --- | --- |
| P01 | [WooCommerce — Enable agentic commerce](https://woocommerce.com/document/woocommerce-ai/agentic-commerce/) | WooCommerce AI 提供 UCP discovery／服務，外部購物平台 onboarding 與支援支付仍另需完成 |
| P02 | [WooCommerce — Claude agent experiment](https://developer.woocommerce.com/2026/09/16/wc-claude-commerce-agent/) | 實驗性 reference 與回原店 checkout；官方明示不是受維護的正式 extension，不能作預設正式交付 |
| P03 | [WooCommerce — Agentic commerce overview](https://woocommerce.com/agentic-commerce/) | 部分 Stripe 功能頁仍寫 coming soon，需與較新的功能文件分開、檢查實際版本 |
| P04 | [BigCommerce — Agentic commerce](https://www.bigcommerce.com/product/agentic-commerce/) | 商品 enrichment 等功能，有 available／early access 區分 |
| P05 | [Feedonomics — Agentic commerce](https://feedonomics.com/product/agentic-commerce/) | 自述商品強化與 AI 通路分發；每個客戶通路、費用、審核另確認 |
| P06 | [Wix — Agentic commerce on Wix](https://www.wix.com/blog/agentic-commerce-on-wix) | 自述平台 partnerships 與購物能力，部分逐步開放 |
| P07 | [Wix — Merchant guide](https://www.wix.com/studio/ai-search-lab/agentic-commerce) | 不同 agent 購物路徑與 Wix 的資料／工具介面；不能據此承諾每個 AI 都會呼叫 |
| P08 | [Shopware — PayPal extension](https://docs.shopware.com/en/shopware-6-en/extensions/paypal) | PayPal Agentic Commerce sales channel；合資格 PayPal 商業帳戶與 plugin 前提 |
| P09 | [Stripe — Sell products through agents](https://docs.stripe.com/agentic-commerce/sellers/use-cases/retail.md) | 管理式 catalog／checkout／支付／訂單；自管與 hooks 的可用階段不同 |
| P10 | [Stripe — Agentic commerce](https://docs.stripe.com/agentic-commerce) | 區分 seller、agent wallet、服務預約與 machine payments；不要混為商品搜尋渠道 |
| P11 | [SHOPLINE — Coming Soon shopping assistant](https://support.shoplineapp.com/hc/en-us/articles/62243748056601--Coming-Soon-AI-Shopping-Assistant-Message-Center) | 查到站內功能預告，不能據此證實外部 AI checkout |
| P12 | [Peec AI](https://peec.ai/) | 供應商自述 AI visibility analytics；未測其覆蓋、成本與準確性 |
| P13 | [Profound — About Shopping](https://help.tryprofound.com/articles/8862399588-about-shopping) | 供應商自述商品卡與商家連結觀測；說明聚焦 ChatGPT Shopping，其他覆蓋演進中 |

## 履約、寄件與售後

| ID | 官方來源 | 支持的判斷／限制 |
| --- | --- | --- |
| L01 | [Shopify — Getting started with Flexport](https://help.shopify.com/en/manual/fulfillment/shopify-fulfillment-network/logistics-partners/flexport-getting-started) | Fulfillment Network app 連結 Flexport、SKU 要求與同步；不是 Shopify 自營倉庫服務的證據 |
| L02 | [ShipBob — Shopify integration](https://partners.shipbob.com/directory/shopify) | Shopify 整合候選 |
| L03 | [ShipBob — Returns API](https://developer.shipbob.com/guides/returns) | 退貨建立、狀態與庫存整合能力；退款仍需另行設計 |
| L04 | [ShipBob — Pricing](https://www.shipbob.com/pricing/) | 客製報價；不能從公開頁推算所有商家固定單價 |
| L05 | [ShipStation — Shopify](https://www.shipstation.com/partners/shopify/) | 訂單、寄件標籤與追蹤整合；不把寄件工具當倉儲 |
| L06 | [Shippo — API](https://goshippo.com/products/api) | 多承運商寄件與退貨標籤工具 |
| L07 | [Easyship — Shopify integration](https://support.easyship.com/hc/en-us/articles/19224078074258-Connect-Your-Shopify-Store) | 訂單同步與即時運價／稅費選項；Shopify 方案限制要再確認 |
| L08 | [Loop — FAQ](https://www.loopreturns.com/faq/) | Shopify／物流與退換貨流程整合，自述功能 |
| L09 | [Loop — Shopify Native Exchanges](https://help.loopreturns.com/en/articles/2771905) | 連回原始訂單的換貨流程；與較舊另開 exchange order 模式分開 |
| L10 | [AfterShip — Returns](https://www.aftership.com/returns) | RMA、規則、標籤、3PL 與狀態整合，自述功能與方案需實際核價 |
| L11 | [ECPay — 物流類型](https://support.ecpay.com.tw/21685/) | 區域備查：台灣宅配／超商與特定亞洲跨境服務；不是美國 3PL 或美國跨境方案證據 |

## 文件差異與尚未關閉的問題

1. **OpenAI 的一般 ACP／Instant Checkout 與 Shopify 的 ChatGPT 通路不同。** A03 的公開規格不會推翻 S02 的導流模式；不能泛稱 Shopify 的 ChatGPT 通路都可 Instant Checkout。
2. **Google 平台範圍與個別 Shopify rollout 不同。** A09／A10 證明整合路徑；S03 與商家後台決定客戶目前能做什麼。網頁／app 也須分開驗收。
3. **WooCommerce 總覽、UCP 功能、實驗範例並非同一種成熟度。** P01 的可設定功能不代表 P02 已獲正式支援；P03 的 coming soon 亦不能直接當所有相關能力皆未上線。
4. **Meta 各 surface 與投放路徑不同。** S08 提及 Meta sales channel，S05 區分 Catalog discovery 與 shoppable ads 同步條件；要依具體 surface 測試，不把 Muse、Facebook ads、Meta AI 全部畫等號。
5. **dots 確認存在，Claude「Do It」未辨識。** 不靠名稱相似就判定為 Cowork；後續取得精確官方名稱／連結再補查。
6. **商家適用性未驗證。** 下一步要確認實際 plan、銷售國、平台帳戶 standing、商品禁限售、checkout 客製與 app 相容性。
7. **供應商價格與責任未確認。** 尚未聯繫廠商、取得報價或簽約，不承諾 3PL 成本、時效、月最低量或 SLA。
8. **營收效益未驗證。** 無本專案客戶樣本，沒有因果增量或付費意願證據；不引用供應商案例的提升比例當我們的預期成果。
