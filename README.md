# 🎨 Text-to-Image Generator

An AI-powered **Text-to-Image Generator** built with **Python and Streamlit** that converts text prompts into images using Hugging Face's Inference API.

The application supports **FLUX.1 Schnell** and **Stable Diffusion XL** models, multiple artistic styles, different image sizes, negative prompts, and PNG image downloads.

---

## ✨ Features

* 📝 Generate images from natural-language text prompts
* 🤖 Supports Hugging Face AI image-generation models
* ⚡ FLUX.1 Schnell for fast, high-quality generation
* 🎨 Stable Diffusion XL support
* 🖌️ Multiple artistic styles:

  * None
  * Photorealistic
  * Anime
  * Digital Art
  * Oil Painting
  * 3D Render
* 📐 Multiple image sizes:

  * 1024 × 1024
  * 768 × 768
  * 512 × 512
  * 1024 × 768
  * 768 × 1024
* 🚫 Optional negative prompts
* 🔐 Hugging Face token entered securely as a password field
* 📥 Download generated images as PNG
* 💻 Simple and beginner-friendly Streamlit interface

---

## 🛠️ Technologies Used

* **Python**
* **Streamlit**
* **Hugging Face Inference API**
* **Hugging Face Hub**
* **FLUX.1 Schnell**
* **Stable Diffusion XL**
* **python-dotenv**
* **Pillow**

---

## 📂 Project Structure

```text
Text-to-Image/
│
├── app.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

### Windows

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
source venv/bin/activate
```

---

## 📦 Install Dependencies

Install the required Python packages:

```bash
pip install streamlit python-dotenv huggingface_hub pillow
```

Or, if you have a `requirements.txt` file:

```bash
pip install -r requirements.txt
```

---

## 🔑 Hugging Face Token

This project requires a **Hugging Face access token** to generate images.

Create an account on Hugging Face and generate a token from your account settings.

You can then enter the token directly in the application's sidebar.

### Recommended: Use `.env`

Create a file named:

```text
.env
```

Add:

```env
HF_TOKEN=your_hugging_face_token
```

The application automatically loads this token using `python-dotenv`.

> ⚠️ Never upload your Hugging Face token to GitHub.

---

## ▶️ Run the Application

Start the Streamlit application using:

```bash
streamlit run app.py
```

The application will open in your browser.

Usually, it will be available at:

```text
http://localhost:8501
```

---

## 🖥️ How to Use

### Step 1: Add Hugging Face Token

Enter your Hugging Face token in the sidebar or configure it using `.env`.

### Step 2: Select a Model

Choose between:

* **FLUX.1 Schnell**
* **Stable Diffusion XL**

### Step 3: Select an Art Style

Choose a style such as:

```text
Photorealistic
Anime
Digital Art
Oil Painting
3D Render
```

### Step 4: Select Image Size

Choose your preferred resolution.

### Step 5: Enter a Prompt

Example:

```text
A cozy tea stall on a rainy evening in Hyderabad, warm lights, cinematic
```

### Step 6: Add a Negative Prompt

Optional example:

```text
blurry, low quality, distorted, bad anatomy
```

### Step 7: Generate

Click:

```text
✨ Generate
```

The AI will generate an image based on your prompt.

### Step 8: Download

Click:

```text
⬇️ Download PNG
```

to save the generated image.

---

## 🧠 Example Prompts

### 🌆 Photorealistic

```text
A futuristic city at night with neon lights, tall skyscrapers and flying cars
```

### 🐱 Anime

```text
A cute cat sitting beside a window while watching the rain
```

### 🏰 Digital Art

```text
A magical castle floating above the clouds at sunset
```

### 🎨 Oil Painting

```text
A peaceful village surrounded by mountains and green fields
```

### 🤖 3D Render

```text
A futuristic AI robot working inside a modern laboratory
```

---

## 🔄 Application Workflow

```text
User enters text prompt
        ↓
Select AI model
        ↓
Select style and image size
        ↓
Optional negative prompt
        ↓
Hugging Face Inference API
        ↓
AI image generation
        ↓
Display generated image
        ↓
Download PNG
```

---

## 📌 Supported Models

### FLUX.1 Schnell

```text
black-forest-labs/FLUX.1-schnell
```

Designed for fast image generation while maintaining high visual quality.

### Stable Diffusion XL

```text
stabilityai/stable-diffusion-xl-base-1.0
```

A popular text-to-image generation model capable of producing detailed images from text prompts.

---

## 📄 requirements.txt

Create a `requirements.txt` file containing:

```text
streamlit
python-dotenv
huggingface_hub
Pillow
```

---

## 🔐 .gitignore

Create a `.gitignore` file:

```text
# Virtual environment
venv/
env/
.venv/

# Environment variables
.env

# Python cache
__pycache__/
*.py[cod]

# Streamlit
.streamlit/secrets.toml

# IDE
.vscode/
.idea/

# OS
.DS_Store
Thumbs.db
```

---

## 🛡️ Security

Do not commit your `.env` file or Hugging Face token.

If your token is accidentally pushed to GitHub:

1. Revoke the exposed token.
2. Generate a new token.
3. Update your `.env` file.
4. Make sure `.env` is included in `.gitignore`.

---

## 🚨 Common Errors

### Token Error

If you see:

```text
Please add your Hugging Face token
```

make sure your token is entered in the sidebar or correctly configured in `.env`.

---

### Model Loading

Sometimes the selected model may take time to load.

Try:

* Waiting for a few seconds
* Trying again
* Selecting another model
* Using a smaller image size

---

### Generation Failed

If image generation fails, check:

* Hugging Face token
* Internet connection
* Model availability
* Selected image size
* Hugging Face service status

---

## 🚀 Future Enhancements

* 🖼️ Generate multiple images at once
* 📚 Maintain image-generation history
* 💾 Save generated images automatically
* 🧑‍🎨 Add more artistic styles
* 🎯 Add advanced generation parameters
* 🖼️ Image-to-image generation
* ✏️ Image editing
* 📱 Improve mobile responsiveness
* ☁️ Deploy the application online
* 👤 Add user accounts and personalized galleries

---

## 🎯 Learning Outcomes

This project demonstrates:

* Python application development
* Streamlit UI development
* Hugging Face model integration
* Generative AI concepts
* API-based AI inference
* Environment-variable management
* Prompt engineering
* Image processing with Pillow
* Building and deploying AI applications

---

## 👩‍💻 Author

**Pravalika Penthala**

B.Tech Computer Science Engineering Student

### Skills Demonstrated

```text
Python
Streamlit
Generative AI
Hugging Face
Prompt Engineering
Machine Learning
API Integration
Git & GitHub
```

---

## ⭐ Project Highlights

> A beginner-friendly Generative AI project that transforms natural-language prompts into AI-generated images using Hugging Face models and a simple Streamlit interface.

If you found this project useful, consider giving the repository a ⭐ on GitHub.
