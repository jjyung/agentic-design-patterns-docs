[English](../17-reasoning-techniques.md) | **繁體中文**

# 17. 推理技術模式 (Reasoning Techniques Pattern)

## 何時使用

- **複雜問題解決**：多步驟邏輯挑戰
- **數學推理**：需要系統性思考的問題
- **策略規劃**：評估多種方法
- **批判性分析**：深入檢視選項
- **決策制定**：系統性權衡替代方案
- **創意探索**：生成多樣化解決方案

## 視覺化流程

```mermaid
graph TD
    Start[困難問題要解決] --> Choose{選擇最佳思考方式}
    
    Choose -->|逐步| StepByStep[逐步思考]
    Choose -->|探索選項| Tree[探索不同路徑]
    Choose -->|再次檢查| Multiple[嘗試多種方式]
    Choose -->|辯論| Debate[辯論雙方]
    Choose -->|思考並執行| ThinkDo[思考然後行動，重複]
    
    StepByStep --> Steps[分解為步驟]
    Steps --> Think1[步驟 1：第一個想法]
    Think1 --> Think2[步驟 2：下一個想法]
    Think2 --> Think3[步驟 3：最終想法]
    
    Tree --> Branch[創建不同想法]
    Branch --> Explore[探索每條路徑]
    Explore --> Compare[比較選項]
    Compare --> Remove[移除不好的路徑]
    
    Multiple --> Make[製作多個解決方案]
    Make --> Path1[解決方案方法 1]
    Make --> Path2[解決方案方法 2]
    Make --> Path3[解決方案方法 3]
    
    Debate --> For[支持論點]
    Debate --> Against[反對論點]
    For --> Discuss[比較論點]
    Against --> Discuss
    
    ThinkDo --> Think[思考它]
    Think --> Act[採取行動]
    Act --> See[看看會發生什麼]
    See --> Think
    
    Think3 --> Grade[評分解決方案]
    Remove --> Grade
    Path1 --> Grade
    Path2 --> Grade
    Path3 --> Grade
    Discuss --> Grade
    
    Grade --> Test{針對標準測試}
    
    Test --> Check[檢查邏輯]
    Check --> Verify[驗證它有效]
    Verify --> Rank[從最佳到最差排名]
    
    Rank --> Pick{選擇贏家}
    
    Pick -->|一個最佳| UseBest[使用最佳解決方案]
    Pick -->|幾個好的| Combine[結合好的部分]
    
    UseBest --> Limit{太多步驟？}
    Combine --> Limit
    
    Limit -->|可以| Continue[繼續]
    Limit -->|太多| Trim[移除額外步驟]
    
    Continue --> Save[儲存工作]
    Trim --> Save
    
    Save --> Keep[保留以供後續使用]
    Keep --> CanReuse[可以再次使用]
    
    CanReuse --> Answer[最終解決方案]
    Answer --> End[問題解決]

    style Start fill:#e1f5fe
    style Choose fill:#fff59d
    style Test fill:#fff9c4
    style Pick fill:#f3e5f5
    style End fill:#c8e6c9
```

## 適用位置

- **研究分析**：分解複雜的研究問題
- **程式碼除錯**：系統性問題識別
- **業務策略**：評估策略選項
- **醫療診斷**：鑑別診斷推理
- **法律分析**：建構邏輯論證

## 優點

- **提高準確性**：系統性思考減少錯誤
- **透明度**：清晰的推理軌跡
- **探索**：考慮多條解決方案路徑
- **健壯性**：多種方法提供驗證
- **學習**：推理軌跡有助於改進
- **彈性**：不同問題使用不同技術
- **品質**：通過深思熟慮獲得更高品質的解決方案

## 缺點

- **延遲增加**：多個推理步驟需要時間
- **標記消耗**：詳細的推理使用更多標記
- **複雜性**：管理推理流程具有挑戰性
- **過度思考**：可能使簡單問題變得複雜
- **上下文限制**：長推理可能超過視窗
- **成本倍增**：多條路徑增加成本
- **收益遞減**：額外推理可能無助益

## 實際案例

1. **數學問題解決器**：
   - 思維鏈逐步解決方案
   - 自我一貫性檢查多種方法
   - 思維樹探索解決方案分支
   - 通過不同方法驗證
   - 清晰的解釋生成

2. **策略性業務顧問**：
   - 思維樹進行策略探索
   - 在成長與效率之間辯論
   - 跨市場分析的自我一貫性
   - 帶資料檢索的 ReAct 模式
   - 最佳策略的綜合

3. **程式碼架構設計師**：
   - 思維鏈用於設計決策
   - 架構的樹探索
   - 設計模式之間的辯論
   - 帶程式碼分析工具的 ReAct
   - 文件的推理持久化

4. **醫療診斷系統**：
   - 鑑別診斷推理樹
   - 跨症狀的自我一貫性
   - 治療計劃的思維鏈
   - 治療選項之間的辯論
   - 基於實證的推理軌跡

5. **法律案例分析器**：
   - 法律論證的思維鏈
   - 先例的樹探索
   - 解釋之間的辯論
   - 跨法規的自我一貫性
   - 結構化法律推理

6. **投資分析平台**：
   - 情境分析的思維樹
   - 跨估值的自我一貫性
   - 多頭與空頭案例的辯論
   - DCF 模型的鏈推理
   - 帶市場資料檢索的 ReAct

## 原始檔案

- **模式討論**：[pattern-discussion/reasoning-techniques.md](../../pattern-discussion/reasoning-techniques.md)
- **Mermaid 來源**：[mermaid-diagrams/reasoning-techniques.mmd](../../mermaid-diagrams/reasoning-techniques.mmd)
