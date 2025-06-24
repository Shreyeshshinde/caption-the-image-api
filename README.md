# 📸 Caption The Image API

A simple API that generates captions for images using a pretrained VisionEncoderDecoderModel (ViT-GPT2) from Hugging Face, built with FastAPI.

---

## 🚀 Features

- Upload an image and get a caption generated.
- Powered by `transformers`, `FastAPI`, and `Docker` for easy deployment.
- Supports GPU acceleration with CUDA.

---

## 🛠️ Tech Stack

- Python
- FastAPI
- Hugging Face Transformers
- ViT-GPT2 (nlpconnect/vit-gpt2-image-captioning)
- Docker (optional for deployment)

---

## 🔧 Setup Instructions

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/caption-the-image-api.git
cd caption-the-image-api
```
2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the FastAPI server
uvicorn app.main:app --reload

4️⃣ Access API Docs
Go to: http://localhost:8000/docs
You can test the API directly from here.

🐳 Docker Deployment (optional)
Build Docker Image:
docker build -t caption-the-image-api .

Run Docker Container:
docker run -p 8000:8000 caption-the-image-api
