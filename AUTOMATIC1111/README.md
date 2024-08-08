# Stable Diffusion web UI
A web interface for Stable Diffusion, implemented using Gradio library.

## Quick Start
- Set `LINK_MODEL` varriable in [SDL](https://github.com/waitrouz/awesome-akash/blob/stable-diffusion-webui/AUTOMATIC1111/deploy.yaml), for a download another model. Current model is ReV Animated v1.2.2
- Deploy on Akash Console using this [SDL](https://github.com/waitrouz/awesome-akash/blob/stable-diffusion-webui/AUTOMATIC1111/deploy.yaml) and open URI after deployment
- After deployment, you can use the `SHELL` tab [Akash Console](https://console.akash.network) to upload additional models, to the `/stable-diffusion-webui/models/Stable-diffusion` folder with command ```bash model LINK_TO_MODEL```

## Documentation
- [AUTOMATIC1111/stable-diffusion-webui on Github](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
- [Rev Animated v1.2.2 on HuggingFace (not official)](https://huggingface.co/danbrown/RevAnimated-v1-2-2)
- [Rev Animated on Civitai](https://civitai.com/models/7371)

## Submission for Akash Zealy
SDL from awesome-akash repository named [AUTOMATIC1111](https://github.com/akash-network/awesome-akash/tree/master/AUTOMATIC1111) with model [rev-animated-v1-2-2.safetensors](https://huggingface.co/danbrown/RevAnimated-v1-2-2)

Example prompt: ```(masterpiece, best quality:1.4), cinematic light, colorful, high contrast, mountain, grass, tree, night, (horror (theme):1.2), (masterpiece, best quality:1.4), (captivating digital art), cinematic lighting, colorful, high contrast, eerie mountain landscape, lush grass, twisted trees, night scene, (horror theme:1.2), (menacing monster:1.2) lurking in shadows, dark atmosphere, blood rain pouring down, blood-red river flowing, haunting blood moon in the sky, chilling and intense visual experience, dark, blood rain, blood river, blood moon, (rating_explicit), (score_9, score_8_up, score_7_up, score_6_up, score_5_up, score_4_up, high res, 4k)```

Output:
![image](https://i.ibb.co/X2hr81q/00003-2949567611.png)
