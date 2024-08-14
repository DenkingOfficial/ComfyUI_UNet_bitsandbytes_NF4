A small modification of the [ComfyUI_bitsandbytes_NF4](https://github.com/comfyanonymous/ComfyUI_bitsandbytes_NF4) extension that allows loading UNet separately from text encoders and VAE.

This may be useful for users who have already downloaded T5, CLIP and VAE to save disk space.

Extension adds UNETLoaderNF4 node (in advanced/loaders category).

NF4 UNet can be obtained [on HuggingFace](https://huggingface.co/duuuuuuuden/flux1-nf4-unet). Download UNet and place it in `ComfyUI/models/unet`.

Requires installing bitsandbytes.

Installation:

* Open terminal in `ComfyUI/custom_nodes` and use this command to clone repo:

    ```git clone https://github.com/DenkingOfficial/ComfyUI_UNet_bitsandbytes_NF4.git```

[Workflow](https://files.catbox.moe/d5ov4n.png)

Original README:

Now on the [manager](https://github.com/ltdrdata/ComfyUI-Manager) for easy installation. Make sure to select Channel:dev in the ComfyUI manager menu or install via git url.

A quickly written custom node that uses code from [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) to support the [nf4 flux dev checkpoint](https://huggingface.co/lllyasviel/flux1-dev-bnb-nf4/blob/main/flux1-dev-bnb-nf4.safetensors) and [nf4 flux schnell checkpoint](https://huggingface.co/silveroxides/flux1-nf4-weights/blob/main/flux1-schnell-bnb-nf4.safetensors).

Requires installing bitsandbytes.

Make sure your ComfyUI is updated.

The node is: CheckpointLoaderNF4, just plug it in your flux workflow instead of the regular one.
