[English](README.md) | **繁體中文**

# Agentic 設計模式文件

一份全面的視覺化與文字文件，涵蓋 21 個建構智能 AI 系統的核心 agentic 設計模式。

## 📚 內容包含

### ⭐ 整合模式 (`/patterns`) - **從這裡開始！**

完整的模式文件，將視覺化圖表和詳細說明整合在一處。每個檔案包含：

- 何時使用該模式
- 互動式 Mermaid 流程圖
- 在架構中的位置
- 優缺點分析
- 實際案例
- 連結至原始檔案

**👉 [瀏覽所有模式](patterns/zh-TW/README.md)**

### 原始文件（依格式分類）

適合偏好分別存取特定格式的使用者：

#### 🔷 Mermaid 圖表 (`/mermaid-diagrams`)

使用簡單英文的視覺化流程圖，展示每個模式的運作方式，設計成無需技術術語即可輕鬆理解。

#### 💬 模式討論 (`/pattern-discussion`)

詳細說明涵蓋：

- 何時使用每個模式
- 在架構中的位置
- 優缺點
- 實作考量

#### 🎨 ASCII 藝術圖表 (`/ascii-art`)

文字式圖表，適合複製到 Miro 看板、文件或任何不支援豐富圖形的地方。

## 🎯 21 個模式

### 核心模式

1. [**提示詞鏈接 (Prompt Chaining)**](patterns/zh-TW/01-prompt-chaining.md) - 將複雜任務分解為連續步驟
2. [**路由 (Routing)**](patterns/zh-TW/02-routing.md) - 將請求導向正確的處理器
3. [**平行化 (Parallelization)**](patterns/zh-TW/03-parallelization.md) - 同時執行多個任務
4. [**反思 (Reflection)**](patterns/zh-TW/04-reflection.md) - 自我評估與改進
5. [**工具使用 (Tool Use)**](patterns/zh-TW/05-tool-use.md) - 整合外部功能

### 進階模式

6. [**規劃 (Planning)**](patterns/zh-TW/06-planning.md) - 策略性任務分解
7. [**多代理協作 (Multi-Agent Collaboration)**](patterns/zh-TW/07-multi-agent-collaboration.md) - 協調多個代理
8. [**記憶體管理 (Memory Management)**](patterns/zh-TW/08-memory-management.md) - 儲存和檢索上下文
9. [**學習與適應 (Learning and Adaptation)**](patterns/zh-TW/09-learning-and-adaptation.md) - 隨時間改進
10. [**模型上下文協定 (Model Context Protocol)**](patterns/zh-TW/10-model-context-protocol.md) - 標準化代理通訊

### 系統模式

11. [**目標設定與監控 (Goal Setting and Monitoring)**](patterns/zh-TW/11-goal-setting-and-monitoring.md) - 追蹤目標
12. [**異常處理與復原 (Exception Handling and Recovery)**](patterns/zh-TW/12-exception-handling-and-recovery.md) - 優雅的錯誤管理
13. [**人工介入 (Human-in-the-Loop)**](patterns/zh-TW/13-human-in-the-loop.md) - 整合人類回饋
14. [**知識檢索 (RAG)**](patterns/zh-TW/14-knowledge-retrieval-rag.md) - 存取外部知識
15. [**代理間通訊 (A2A)**](patterns/zh-TW/15-inter-agent-communication-a2a.md) - 代理對代理訊息傳遞

### 最佳化模式

16. [**資源感知最佳化 (Resource-Aware Optimization)**](patterns/zh-TW/16-resource-aware-optimization.md) - 高效資源使用
17. [**推理技術 (Reasoning Techniques)**](patterns/zh-TW/17-reasoning-techniques.md) - 結構化思考方法
18. [**護欄/安全模式 (Guardrails/Safety Patterns)**](patterns/zh-TW/18-guardrails-safety-patterns.md) - 確保安全運作
19. [**評估與監控 (Evaluation and Monitoring)**](patterns/zh-TW/19-evaluation-and-monitoring.md) - 效能追蹤

### 策略模式

20. [**優先順序 (Prioritization)**](patterns/zh-TW/20-prioritization.md) - 管理任務重要性
21. [**探索與發現 (Exploration and Discovery)**](patterns/zh-TW/21-exploration-and-discovery.md) - 尋找新解決方案

## 🚀 快速開始

**建議**：從[**整合模式目錄**](patterns/zh-TW/README.md)開始，獲得完整體驗。

每個整合模式檔案包含：

- 使用指引
- 展示流程的視覺化 Mermaid 圖表
- 在架構中的位置
- 優缺點分析
- 詳細範例的實際使用案例
- 原始檔案參考

**替代方案**：如果偏好分別存取特定格式，可導覽至個別資料夾（[mermaid-diagrams](mermaid-diagrams/)、[pattern-discussion](pattern-discussion/)、[ascii-art](ascii-art/)）。

## 📖 來源

這些模式是從關於 agentic AI 系統的廣泛研究中提煉而來，透過簡單的視覺化呈現和清晰的說明使其易於理解。

## 🤝 貢獻

歡迎透過 issues 或 pull requests 提出改進建議或補充模式。

## 📄 授權

MIT 授權 - 在您的專案中自由使用這些模式！
