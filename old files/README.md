# 🎙️ Welcome to Your Custom RVC Voice Conversion Model!

This project uses the Retrieval-based Voice Conversion (RVC) system through a user-friendly web-based GUI hosted in Google Colab. With your trained model, you can convert any voice into your custom target voice.

---

## 1️⃣ - How to Use the Google Colab Notebook

1. **Clone the IPython file into a new Colaboratory session**

   [![](https://img.shields.io/static/v1?message=Open%20in%20Colab&logo=googlecolab&labelColor=5c5c5c&color=0f80c1&label=%20&style=for-the-badge)](https://colab.research.google.com/github/zzryn/rvc-webui/blob/main/rvc-webui.ipynb)

1. ***Do not*** change any pre-configured options, as everything is already set up for you.

2. Run each cell by clicking the ▶️ play buttons on the left side of every code cell, starting from the first.

4. **Be patient!** Some steps (like environment setup or model loading) may take a ~~minute or two~~ fuck ton of time.

5. Once you see this message:

```
Running on public URL: https://**************.gradio.live
```

Click that link to open the RVC web interface in a new tab.

---

## 2️⃣ - Using the Web Interface for Inference

### 1. Load Your Model
- Use the **Model** dropdown at the top to select your trained voice model.

### 2. Add Source Audio
- Enter the path or drag & drop the audio file you want to convert into the **Source Audio** field.

### 3. Set Output Location
- Default is `/content/rvc-webui/outputs`, but you can modify it as needed.

### 4. Customize Settings (Optional)
- **Transpose**: Shift pitch (positive = higher, negative = lower).
- **Pitch Extraction Algorithm**: Recommended default is `crepe`.
- **Embedder Model**: Keep `auto` unless using a specific model (e.g., `hubert-base-japanese`).
- **Embedder Output Layer**: Leave as `auto`, or choose a specific layer like `9` or `12`.

### 5. (Optional) Use Retrieval Features
- Enable **Auto Load Index** if applicable.
- Set **Faiss Index File Path** and **Retrieval Feature Ratio**.
- You can also upload an **F0 Curve File** to control pitch curves directly.

### 6. Run Inference
- Hit the bright **Infer** button at the bottom.
- Your converted audio will be saved in the specified output folder and listed under the "Output" section.

---

## 📂 Output Location
Converted files are stored in the output folder and can be played or downloaded directly from the web UI.

---

## 🙋 Need Support?
If anything breaks or you get lost, first check out the [official RVC GitHub repo](https://github.com/RVC-Project) to see if your problem can be resolved there. Alternatively, use [our issues page](https://github.com/zzryn/rvc-webui/issues) to report a problem; but ***please*** post a **detailed** report otherwise I might not be able to help resolve an issue.
