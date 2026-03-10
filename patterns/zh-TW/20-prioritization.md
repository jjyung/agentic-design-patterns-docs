[English](../20-prioritization.md) | **繁體中文**

# 20. 優先順序模式 (Prioritization Pattern)

## 何時使用

- **資源約束**：有限的處理能力
- **多個目標**：競爭的目標和任務
- **動態環境**：不斷變化的優先順序
- **複雜依賴**：具有相互依賴的任務
- **時間敏感操作**：截止日期驅動的工作
- **公平排程**：防止任務飢餓

## 視覺化流程

```mermaid
graph TD
    Start[任務佇列] --> Build[建構依賴圖]
    
    Build --> Map[對映依賴]
    Map --> Tasks[任務清單]
    Tasks --> T1[任務 1]
    Tasks --> T2[任務 2]
    Tasks --> T3[任務 3]
    Tasks --> TN[任務 N]
    
    T1 --> Score[為每個任務評分]
    T2 --> Score
    T3 --> Score
    TN --> Score
    
    Score --> Value{評分因素}
    
    Value --> Business[業務價值]
    Value --> Risk[風險等級]
    Value --> Effort[所需努力]
    Value --> Urgency[時間敏感性]
    Value --> Dependencies[依賴數量]
    
    Business --> Calculate[計算優先順序分數]
    Risk --> Calculate
    Effort --> Calculate
    Urgency --> Calculate
    Dependencies --> Calculate
    
    Calculate --> Formula[優先順序 = 價值/努力 × 緊急性 × 風險]
    
    Formula --> Rank[排序任務]
    Rank --> Order[初始順序]
    
    Order --> Schedule{排程策略}
    
    Schedule --> Quota[應用配額]
    Schedule --> Aging[任務老化]
    Schedule --> Balance[負載平衡]
    
    Quota --> Prevent[防止飢餓]
    Aging --> Boost[提升舊任務]
    Balance --> Distribute[分配工作]
    
    Prevent --> Queue2[優先順序佇列]
    Boost --> Queue2
    Distribute --> Queue2
    
    Queue2 --> Execute[執行最高優先任務]
    
    Execute --> Monitor{新的高優先順序？}
    
    Monitor -->|是| Preempt[搶佔當前]
    Monitor -->|否| Continue[繼續當前]
    
    Preempt --> Save[儲存狀態]
    Save --> Switch[切換到高優先順序]
    
    Continue --> Complete{任務完成？}
    Switch --> Complete
    
    Complete -->|是| Remove[從佇列移除]
    Complete -->|否| Execute
    
    Remove --> Events{新事件？}
    
    Events -->|是| Reorder[重新計算優先順序]
    Events -->|否| Next[取得下一個任務]
    
    Reorder --> Rank
    Next --> Execute
    
    Next --> End[最佳化執行]

    style Start fill:#e1f5fe
    style Value fill:#fff59d
    style Schedule fill:#fff9c4
    style Monitor fill:#f3e5f5
    style End fill:#c8e6c9
```

## 適用位置

- **任務管理系統**：工作流程編排
- **客戶服務**：工單優先順序
- **製造**：生產排程
- **醫療**：患者分流系統
- **DevOps**：部署和維護優先順序

## 優點

- **效率**：資源的最佳使用
- **回應性**：優先處理高優先順序項目
- **公平性**：防止無限期延遲
- **適應性**：調整以適應變化條件
- **透明度**：清晰的優先順序邏輯
- **目標一致**：按業務價值排序任務
- **可擴展性**：處理增長的任務佇列

## 缺點

- **複雜性**：優先順序計算可能很複雜
- **開銷**：持續重新排序消耗資源
- **飢餓風險**：低優先順序任務可能永遠等待
- **上下文切換**：搶佔增加開銷
- **主觀評分**：優先順序因素可能有爭議
- **依賴**：複雜的依賴管理
- **預測錯誤**：努力估計可能錯誤

## 實際案例

1. **客戶支援系統**：
   - 高級客戶獲得優先權
   - 緊急問題排名較高
   - 基於年齡的升級
   - 基於技能的路由
   - SLA 合規追蹤
   - 代理之間的負載平衡

2. **軟體開發管線**：
   - 關鍵錯誤優先處理
   - 功能價值評分
   - 技術債務排程
   - 依賴解決
   - 衝刺容量規劃
   - 資源分配

3. **醫療分流**：
   - 緊急嚴重程度評分
   - 等待時間考慮
   - 資源可用性
   - 專家路由
   - 測試結果優先順序
   - 預約排程

4. **製造排程器**：
   - 訂單價值優先順序
   - 截止日期管理
   - 資源最佳化
   - 設定時間最小化
   - 品質需求
   - 維護視窗

5. **內容發佈**：
   - 熱門主題優先權
   - 編輯日曆
   - 作者可用性
   - SEO 價值評分
   - 社群媒體時機
   - 跨平台協調

6. **網路流量管理**：
   - QoS 封包優先順序
   - 頻寬分配
   - 延遲敏感路由
   - 公平排隊
   - 緊急流量優先權
   - 負載平衡

## 原始檔案

- **模式討論**：[pattern-discussion/prioritization.md](../../pattern-discussion/prioritization.md)
- **Mermaid 來源**：[mermaid-diagrams/prioritization.mmd](../../mermaid-diagrams/prioritization.mmd)
