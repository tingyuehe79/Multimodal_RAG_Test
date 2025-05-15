# Multimodal_RAG_Test
## 本地最小化部署 多模态RAG
### 目标：
- 文本提问 + 图像上下文 + LLM生成回答
- 可以一站式本地跑通，不需要云服务
### 部署技术选型
- 模型： Qwen-VL-Chat（图文理解 + 生成）
- RAG 流程控制： python 脚本
- 向量检索（可选）：CLIP + FAISS（如要做大规模图像检索，此版本没得）
### 部署结构设计 Project Structure
- `multimodal_rag/`
  - `images/` — Place your test images here
    - `your_image.jpg`
  - `docs/` — Optional: Place your knowledge base text files here
    - `your_doc.txt`
  - `rag_runner.py` — Main RAG runner script
  - `requirements.txt` — Python dependency list
  - `README.md` — Project documentation

### this version offers requirement.txt
torch
transformers
accelerate
sentencepiece
pillow
