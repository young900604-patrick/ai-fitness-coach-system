# AI 健身教練系統（AI Fitness Coach System）

本專案為一套基於大型語言模型（Large Language Model, LLM）的智慧健身教練系統，透過自然語言互動，提供即時且個人化的運動建議與訓練指導。

本系統旨在解決傳統健身應用程式缺乏互動性與個人化建議的問題，讓使用者能像與真人教練對話般，隨時獲得專業回饋。

---

## 🔥 系統特色（Features）

- 即時互動：透過 WebSocket 實現低延遲雙向通訊  
- 個人化建議：根據使用者問題提供客製化健身建議  
- 自然語言問答：支援訓練動作、課表安排與運動觀念詢問  
- 模擬真人教練：提升使用者學習體驗與互動感  
- 輕量化模型應用：採用 LoRA 微調之小型 LLM（Gemma 3-1B）

---

## 🧠 系統架構（System Architecture）

本系統採用三層式架構設計：

- 前端介面（Frontend UI）：HTML / CSS / JavaScript  
- 後端服務（Backend Service）：ASP.NET MVC（C#）  
- 模型推論伺服器（LLM Inference Server）：Python  

系統透過 WebSocket 建立即時通訊管道，使用者問題由前端送至後端，再轉送至模型推論伺服器，並將生成結果即時回傳顯示。

---

## ⚙️ 使用技術（Technologies）

- ASP.NET MVC（C#）
- WebSocket 即時通訊
- Python / PyTorch
- LoRA 微調技術（Low-Rank Adaptation）
- Gemma 3-1B 大型語言模型
- HTML / CSS / JavaScript
- PostgreSQL（資料庫）
- Railway（雲端部署）

---

## 🧪 模型微調實作（Model Fine-tuning）

本專案使用 Gemma 3–1B 輕量化大型語言模型，並透過 LoRA（Low-Rank Adaptation）進行領域微調。

訓練過程中使用自建健身語料資料集（JSONL 格式），將健身知識有效注入模型中，使其能針對訓練問題提供更具專業性的回應。

以下為實際微調程式碼設定範例：

![LoRA Training](lora_training.png)

---

## ⚡ 系統設計理念（Lightweight Design）

本專案特別強調「輕量化（Lightweight）」設計，在有限硬體資源下，透過小型模型（Gemma 3–1B）與 LoRA 微調技術，實現具實用價值的 AI 系統。

相較於大型模型需高運算成本，本系統著重於：

- 降低模型運算需求  
- 提升系統可部署性  
- 維持合理回應品質  

此設計展現了模型效能與系統效率之間的工程取捨（trade-off），使系統更適合部署於資源受限環境（resource-constrained environments），並具備實際應用潛力。

---

## 🤖 模型連結（Hugging Face）

👉 已將微調後模型部署於 Hugging Face：

https://huggingface.co/TsaiPatrick64/ai-fitness-coach-lora

使用者可透過該連結查看模型成果與實際應用效果。

---

## 💡 專案說明（Description）

本專案透過人工智慧技術模擬真人健身教練，使用者可針對以下情境進行提問：

- 訓練動作與姿勢修正  
- 每週訓練課表安排  
- 運動觀念與基礎知識  
- 運動過程中不適與疑問  

系統能即時理解問題並生成對應建議，有效提升訓練效率並降低受傷風險。

---

## 🚀 未來發展（Future Work）

- 整合姿態辨識（Pose Estimation）技術  
- 支援語音互動（Voice Interaction）  
- 結合穿戴裝置數據（心率、睡眠）  
- 開發行動裝置 App  
- 強化多模態輸入（影像 + 語音）

---

## 📌 專案價值（Project Impact）

本專案展示了大型語言模型在健康與運動領域的應用潛力，並透過輕量化設計，使 AI 技術能更貼近實際使用場景。

透過智慧健身教練系統，可有效降低健身門檻，提供即時且個人化的運動指導，促進使用者建立健康生活習慣。
