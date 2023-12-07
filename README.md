# Real-time-Img2img-translation (TouchDesigner + T2Iadapter_canny + SDXL + turbo_LoRA) 

I used the 'Touch Designer' tool to create videos in near-real time by translating user movements into img2img translation! It only takes about 0.2 to 0.5 seconds to create a single frame. The ability to produce high-quality videos in real time is thanks to SDXL turbo. Using the LoRA model, you can produce high-quality images very quickly with just about 2 steps, regardless of which SDXL ckpt you use.

To maintain consistency, I initially intended to use ControlNet. However, ControlNet takes longer because it needs to be loaded into the network each time. So, I solved this problem by using the T2I Adapter. In this video, I used Canny, but if more Adapters are released for the SDXL version (such as recolor), I expect even better results.

I've also tried [ControlLoRA](https://huggingface.co/stabilityai/control-lora), [ControlNet+LCM_LoRA](https://www.youtube.com/watch?v=icZze060TiE), [ControlNet-LLLite](https://github.com/kohya-ss/ControlNet-LLLite-ComfyUI), but **T2I adapter + SDXL-turbo-LoRA** was the best solution. 

Check out [my github page](https://github.com/AllenEdgarPoe) if you want to view my experiment results! (SORRY, I'M ON VACATION RIGHT NOW SO I'LL UPDATE THE DETAILS AS SOON AS I COMEBACK) 


### Acknowledgement
- This project is done in my company [XORBIS](https://xorbis.com). 
- [SDXL Turbo-LoRA] (https://civitai.com/models/215485/sdxl-turbo-lora-stable-diffusion-xl-faster-than-light)
- [T2I adapter] (https://huggingface.co/spaces/TencentARC/T2I-Adapter-SDXL)
