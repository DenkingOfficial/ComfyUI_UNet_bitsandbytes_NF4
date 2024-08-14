A small modification of the [ComfyUI_bitsandbytes_NF4](https://github.com/comfyanonymous/ComfyUI_bitsandbytes_NF4) extension that allows loading UNet separately from text encoders and VAE

This may be useful for users who have already downloaded T5, CLIP and VAE to save disk space

NF4 UNet can be obtained [on HuggingFace](https://huggingface.co/duuuuuuuden/flux1-nf4-unet)

Extension adds UNETLoaderNF4 node (in advanced/loaders category)

Original README:

Now on the [manager](https://github.com/ltdrdata/ComfyUI-Manager) for easy installation. Make sure to select Channel:dev in the ComfyUI manager menu or install via git url.

A quickly written custom node that uses code from [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) to support the [nf4 flux dev checkpoint](https://huggingface.co/lllyasviel/flux1-dev-bnb-nf4/blob/main/flux1-dev-bnb-nf4.safetensors) and [nf4 flux schnell checkpoint](https://huggingface.co/silveroxides/flux1-nf4-weights/blob/main/flux1-schnell-bnb-nf4.safetensors).

Requires installing bitsandbytes.

Make sure your ComfyUI is updated.

The node is: CheckpointLoaderNF4, just plug it in your flux workflow instead of the regular one.
