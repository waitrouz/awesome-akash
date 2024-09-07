# ComfyUI on Akash Network
This UI will let you design and execute advanced stable diffusion pipelines using a graph/nodes/flowchart based interface. For some workflow examples and see what ComfyUI can do you can check out [ComfyUI Examples](https://comfyanonymous.github.io/ComfyUI_examples/)

Env variables MODELURLS (checkpoints), VAEURLS (vae) and UPSCALEURLS (upscale_model) can be set to automatically download models on deployment start. Just add a string with download urls separated by ","

COMMANDLINE_ARGS can be found [here](https://github.com/comfyanonymous/ComfyUI/blob/9bfec2bdbf0b0d778087a9b32f79e57e2d15b913/comfy/cli_args.py#L36)

## Install flux1-schnell model on ComfyUI
1. Deploy ComfyUI on Akash Console using `deploy.yaml` file from this repository.
2. Open Shell tab on Akash Console and download flux1-schnell model (unet, vae, clip).
```
wget https://huggingface.co/black-forest-labs/FLUX.1-schnell/resolve/main/flux1-schnell.safetensors -P /comfyui/models/unet
wget https://huggingface.co/black-forest-labs/FLUX.1-schnell/resolve/main/ae.safetensors -P /comfyui/models/vae
wget https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/main/clip_l.safetensors -P /comfyui/models/clip
wget https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/main/t5xxl_fp16.safetensors -P /comfyui/models/clip
```
Minimum hardware requirements for these models: 24GB VRAM, 32GB RAM.

3. Look at Leases tab and open link under port 8080.
4. Use ComfyUI manager to update software and node. Click `Update all` button and restart application after updating.
5. Look at Custom Nodes Manager. Update `ComfyUI-Manager` and restart application after updating.
6. Look at workflow for flux1-schnell [here](https://comfyanonymous.github.io/ComfyUI_examples/flux/#flux-schnell). Drag and drop image from this link into your ComfyUI app.
7. Write your prompt in `CLIP Text Encode (Prompt)` node and click `Queue Prompt` button to generate an image from text.

## Showcase

Example prompt:
`a bottle with a beautiful rainbow galaxy inside it on top of a wooden table in the middle of a modern kitchen beside a plate of vegetables and mushrooms and a wine glasse that contains a planet earth with a plate with a half eaten apple pie on it`

Output:
![Comfy-UI-00004](https://github.com/user-attachments/assets/891c3d40-528d-4ffe-91d7-b2357f8b0a76)
