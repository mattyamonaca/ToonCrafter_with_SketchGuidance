## ___***ToonCrafter_with_SketchGuidance***___


https://github.com/user-attachments/assets/f72f287d-f848-4982-8f91-43c49d037007



## 🧰 Models

|Model|Resolution|GPU Mem. & Inference Time (A100, ddim 50steps)|Checkpoint|
|:---------|:---------|:--------|:--------|
|ToonCrafter_512|320x512| TBD (`perframe_ae=True`)|[Hugging Face](https://huggingface.co/Doubiiu/ToonCrafter/blob/main/model.ckpt)|
|ToonCrafter_512|TBD| TBD |[Hugging Face](https://huggingface.co/Doubiiu/ToonCrafter/blob/main/sketch_encoder.ckpt)|


Currently, our ToonCrafter can support generating videos of up to 16 frames with a resolution of 512x320. The inference time can be reduced by using fewer DDIM steps.



## ⚙️ Setup

### Install Environment via Anaconda (Recommended)
```bash
conda create -n tooncrafter python=3.8.5
conda activate tooncrafter
pip install -r requirements.txt
```


## 💫 Inference

### 1. Local Gradio demo

Download the pretrained model and put it in the corresponding directory according to the previous guidelines.
```bash
  python gradio_app.py 
```
