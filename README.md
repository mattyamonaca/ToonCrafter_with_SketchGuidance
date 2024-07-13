## ___***ToonCrafter_with_SketchGuidance***___
This repository is an implementation that recreates the SketchGuidance feature of "ToonCrafter".

- https://github.com/ToonCrafter/ToonCrafter
- https://arxiv.org/pdf/2405.17933

https://github.com/user-attachments/assets/f72f287d-f848-4982-8f91-43c49d037007



## 🧰 Models

|Model|Resolution|GPU Mem. & Inference Time (A100, ddim 50steps)|Checkpoint|
|:---------|:---------|:--------|:--------|
|ToonCrafter_512|320x512| TBD (`perframe_ae=True`)|[Hugging Face](https://huggingface.co/Doubiiu/ToonCrafter/blob/main/model.ckpt)|
|SketchEncoder|TBD| TBD |[Hugging Face](https://huggingface.co/Doubiiu/ToonCrafter/blob/main/sketch_encoder.ckpt)|


Currently, ToonCrafter can support generating videos of up to 16 frames with a resolution of 512x320. The inference time can be reduced by using fewer DDIM steps.



## ⚙️ Setup

### Install Environment via Anaconda (Recommended)
```bash
conda create -n tooncrafter python=3.8.5
conda activate tooncrafter
pip install -r requirements.txt
```


## 💫 Inference

### 1. Local Gradio demo
1. Download pretrained ToonCrafter_512 and put the model.ckpt in checkpoints/tooncrafter_512_interp_v1/model.ckpt.
2. Download pretrained SketchEncoder and put the model.ckpt in control_models/sketch_encoder.ckpt.

```bash
  python gradio_app.py 
```
