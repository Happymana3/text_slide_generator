# 📊 AI Slide Generator

This Streamlit app allows you to **automatically generate PowerPoint slides** from `.txt`, `.pdf`, or `.xlsx` files using a Hugging Face summarization model. Built entirely within **Google Colab** with an easy-to-use interface.

---

## 🚀 Features

- ✅ Upload `.txt`, `.pdf`, or `.xlsx` files  
- 🧠 AI-generated slide content using `facebook/bart-large-cnn`  
- 🎨 Beautiful slide formatting with custom fonts, colors, and bullets  
- 📥 Download `.pptx` slides instantly  
- 🔒 Secure token-based setup for pushing updates  

---

## 🛠️ Tech Stack

- **Frontend**: [Streamlit](https://streamlit.io/)  
- **NLP Model**: [`facebook/bart-large-cnn`](https://huggingface.co/facebook/bart-large-cnn)  
- **Slide Generation**: `python-pptx`  
- **Cloud Hosting**: Google Colab + Ngrok  
- **Version Control**: GitHub  

---

## 📂 How to Run

1. Clone the repo (or open in Colab):
    ```bash
    !git clone https://github.com/Happymana3/text_slide_generator.git
    %cd text_slide_generator
    ```

2. Open or upload your `app.py` to Google Colab.

3. Install dependencies (in Colab):
    ```python
    !pip install streamlit transformers pyngrok python-pptx PyPDF2 pandas
    ```

4. Start the app using ngrok:
    ```python
    from pyngrok import ngrok
    !streamlit run app.py &
    public_url = ngrok.connect(port='8501')
    print(public_url)
    ```

---

## 🔐 Security

To keep your `pyngrok` or GitHub API keys safe, store them in environment variables instead
