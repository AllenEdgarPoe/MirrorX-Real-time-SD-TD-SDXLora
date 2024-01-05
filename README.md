# Real-time-Img2img-translation (TouchDesigner + T2Iadapter_canny + SDXL + turbo_LoRA) 


https://github.com/AllenEdgarPoe/Real-time-SD-TD-SDXLora/assets/43398106/659e2d0d-31dd-4c72-a8fc-0eb70f085a42


I used the 'Touch Designer' tool to create videos in near-real time by translating user movements into img2img translation! It only takes about 0.2 to 0.5 seconds to create a single frame. The ability to produce high-quality videos in real time is thanks to SDXL turbo. Using the LoRA model, you can produce high-quality images very quickly with just about 2 steps, regardless of which SDXL ckpt you use.

To maintain consistency, I initially intended to use ControlNet. However, ControlNet takes longer because it needs to be loaded into the network each time. So, I solved this problem by using the T2I Adapter. In this video, I used Canny, but if more Adapters are released for the SDXL version (such as recolor), I expect even better results.

I've also tried [ControlLoRA](https://huggingface.co/stabilityai/control-lora), [ControlNet+LCM_LoRA](https://www.youtube.com/watch?v=icZze060TiE), [ControlNet-LLLite](https://github.com/kohya-ss/ControlNet-LLLite-ComfyUI), but **T2I adapter + SDXL-turbo-LoRA** was the best solution. 

## How to Do
1. Download [ComfyUI] (https://github.com/comfyanonymous/ComfyUI), enable API settings.
2. Connect your pc with webcam, and uisng TouchDesigner, send the images to ComfyUI via API.
3. Copy workflow from `jsong_files` and play around!


https://www.reddit.com/r/StableDiffusion/comments/18cnyo7/realtime_img2img_translation/


## Updates
* [2023-01-05] Updated TDComfyUI.tox file from [TouchDesigner SD] (https://github.com/olegchomp/TDComfyUI) and 'HOW TO DO' in README.md
* [2023-12-18] Updated ComfyUI workflow 


---


### Acknowledgement
- This project is done in my company [XORBIS](https://xorbis.com), with my co-worker (https://github.com/jms-storage). He is the coolest artist-technician using TouchDesigner! 
- [SDXL Turbo-LoRA] (https://civitai.com/models/215485/sdxl-turbo-lora-stable-diffusion-xl-faster-than-light)
- [T2I adapter] (https://huggingface.co/spaces/TencentARC/T2I-Adapter-SDXL)
