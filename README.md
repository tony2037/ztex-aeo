# ZTEX AEO

目前聚焦美國市場中會開團購的小型網紅／團主，探索如何簡化開團、訂單管理、客服、退換貨與供應商對帳。專案 owner：Tony Liu；目前階段：需求研究與試點設計，尚未驗證付費意願。

原始構想為中小型品牌的 AI 搜尋與電商整合服務。以下研究文件保留這段探索背景，尚未全面改寫為團購產品規格；目前方向以 [MEMORY.md](MEMORY.md) 為準。

## 從這裡開始

- [深度研究與商業建議](docs/research/2026-10-31-us-agentic-commerce.md)：定位、客群、平台、agent、物流、競爭與收費。
- [服務交付流程](docs/service-pipeline.md)：每個步驟的工作、產出與驗收。
- [90 天驗證計畫](docs/roadmap.md)：先驗證付費需求，再決定產品化。
- [官方來源與查證紀錄](docs/research/sources.md)：能力邊界、文件差異與待確認問題。
- [商家訪談與資料表](templates/merchant-intake.md)、[曝光實驗紀錄](templates/visibility-run.md)。

## 專案背景

[MEMORY.md](MEMORY.md) 保存專案背景與決策；[CLAUDE.md](CLAUDE.md) 與 [AGENTS.md](AGENTS.md) 指向它。

第一階段以美國市場為準。已有 Shopify 商店不是招募門檻；優先了解團主現有的接單方式、廠商合作條件與售後負擔，再選擇電商、付款和客服整合。實作仍需相關業者授權帳號，確認收款、出貨、退款與對帳責任。

## Repository 狀態

Git 使用 `main` 分支；遠端 repository 為 [tony2037/ztex-aeo](https://github.com/tony2037/ztex-aeo)，SSH 位址為 `git@github.com:tony2037/ztex-aeo.git`。現階段是研究與服務設計 repository，尚無應用程式、部署環境或客戶實測數據。

機密、客戶原始資料、訂單與付款資訊不得放進 Git。可分享的研究與去識別化範本才放在此處。
