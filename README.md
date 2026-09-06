# ⚡ Z Image Turbo with LoRA in Google Colab

This repository contains an easy-to-use Google Colab notebook for running **Z-Image Turbo Q8_0 GGUF** powered by ComfyUI. It allows you to generate high-quality AI images extremely fast using the Qwen text encoder and VAE, with built-in support for GGUF nodes and custom LoRAs.

**🎥 Watch the Tutorial:** [How to Use Z Image Turbo](https://www.youtube.com/watch?v=8q3HMyMpxn8)

**🚀 Run in Colab:** [Open Google Colab Notebook](https://colab.research.google.com/drive/1NE0mEqYx8wcuBnN9MTxv67uGoQUrLIrv?usp=sharing)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salman02-12/Z-Image-Turbo-with-LoRA-in-Google-Colab/blob/main/Z_Image_Turbo_CoinNoin.ipynb)

---

## ✨ Features Supported in this Notebook

The notebook is divided into 3 automated steps to get you generating images quickly:

1. **⚙️ Initialize Core Environment**: Installs ComfyUI and configures the essential GGUF processing nodes.
2. **📥 High-Speed Asset Downloader & LoRA Setup**: Uses Aria2c to rapidly download the fixed Z-Image Turbo Q8_0 GGUF UNet, Qwen text encoders, and VAE. It also features options to easily download a LoRA via URL or upload one directly from your computer.
3. **🎨 Image Generation**: Generate images using a fully integrated workflow. Features include:
   * **Prompts**: Enter positive and negative text prompts, plus LoRA trigger words.
   * **Model & LoRA Selection**: Run in pure base model mode, manually type your LoRA filename, or use "auto" to detect the most recent one.
   * **Dimensions & Batches**: Sliders for width, height, and batch size.
   * **Advanced Sampler Settings**: Tweak Steps, CFG, Aura Shift, and choose from a massive list of Samplers (e.g., `euler`, `dpmpp_2m_sde_gpu`) and Schedulers (e.g., `beta`, `karras`).
   * **Auto-download**: Option to automatically download the finished image locally.

## 🛠️ How to Use

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type** and ensure a **T4 GPU** is selected.
3. Run **Cell 1** to initialize the ComfyUI core engine.
4. Go to **Cell 2**. Select your `LORA_SOURCE` (None, Download from URL, or Upload from Computer), paste the URL if applicable, and run the cell to download all assets. Take note of the listed "Available LoRAs in storage" at the bottom of the output.
5. Go to **Cell 3**. Type your LoRA filename (or use "auto"/"None"), enter your prompts, tweak the settings (Steps, Sampler, etc.), and hit Play. The ComfyUI server will start in the background, and your generated image will appear below the cell!

## 🤝 Credits
* **Notebook Creator:** [CoinNoin](https://www.youtube.com/@CoinNoin)
* **Base Model (GGUF):** [Unsloth / Z-Image-Turbo-GGUF](https://huggingface.co/unsloth/Z-Image-Turbo-GGUF)
