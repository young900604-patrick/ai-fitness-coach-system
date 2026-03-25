# AI 健身教練系統（AI Fitness Coach System）

本專案為一套基於大型語言模型（LLM）的智慧健身教練系統，透過自然語言互動，提供即時且個人化的運動建議與訓練指導。

---

## 🔥 系統特色（Features）

- 透過 WebSocket 實現即時雙向互動
- 提供個人化健身建議
- 支援自然語言問答（Q&A）系統
- 採用 LoRA 微調之大型語言模型（Gemma 3-1B）

---

## 🧠 系統架構（System Architecture）

本系統採用三層式架構設計：

- 前端介面（Frontend UI）：HTML / CSS / JavaScript  
- 後端服務（Backend Service）：ASP.NET MVC  
- 模型推論伺服器（LLM Inference Server）：Python  

---

## ⚙️ 使用技術（Technologies）

- ASP.NET MVC（C#）
- WebSocket 即時通訊
- Python / PyTorch
- LoRA 微調技術（LoRA Fine-tuning）
- Gemma 3-1B 大型語言模型

---

## 🤖 模型連結（Hugging Face）

https://huggingface.co/TsaiPatrick64/ai-fitness-coach-lora

---

## 💡 專案說明（Description）

本專案旨在透過人工智慧技術，模擬真人健身教練的互動方式。使用者可以針對訓練安排、動作姿勢修正或健身相關問題進行提問，系統將即時生成對應建議。

本系統改善了傳統健身應用程式缺乏互動與個人化的問題，提供更即時且具情境理解能力的運動指導，提升使用者的學習效率與訓練體驗。
