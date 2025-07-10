# txt-to-img_AI

# Text-to-Image Generation Notebook

![Stable Diffusion Example](generated_image_example.png) <!-- Optional header image -->

This Jupyter Notebook provides an interactive interface for generating images from text prompts using **Stable Diffusion models** from Hugging Face. It runs on Google Colab with GPU acceleration.

## Features
- 🎨 Generate images from text descriptions
- ⚙️ Choose between Stable Diffusion 1.5 or XL models
- ⏱️ Select different schedulers for generation
- 🔒 Secure Hugging Face token input
- 🚀 GPU-accelerated inference

## Prerequisites
1. **Hugging Face Account**  
   [Sign up here](https://huggingface.co/join) if you don't have one
2. **Access Token**  
   Get your token from [Hugging Face Settings > Access Tokens](https://huggingface.co/settings/tokens)

## Setup Instructions
1. **Open in Google Colab**  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-repo/your-notebook)
   (Upload the notebook to Colab)

2. **Select GPU Runtime**  
   `Runtime` → `Change runtime type` → Select `T4 GPU`

3. **Enter Hugging Face Token**  
   Paste your token in the "HF Token" field when prompted

## Usage Guide
### 1. Configuration Options
- **Model Selection**:
  - `Stable Diffusion 1.5`: Faster generation
  - `Stable Diffusion XL`: Higher quality results
  
- **Scheduler Options**:
  - `DDIM` - Denoising Diffusion Implicit Models
  - `DPMSolverMultistep` - Fast high-order solver
  - `LMSDiscrete` - Linear Multistep Scheduler
  - `Custom` - Custom configuration

### 2. Enter Your Prompt
Type your image description in the "Prompt" field.  
Example: `"A serene castle floating in clouds"`

### 3. Generate Image
Click the 🚀 **Generate** button to create your image

## Technical Details
- **Backend**: Uses Hugging Face `diffusers` library
- **Hardware**: Requires GPU (T4 recommended)
- **Security**: Token is hidden during input
- **Output**: 1024x1024 resolution images

## Example Prompts
Try these sample prompts:
- "Cyberpunk cityscape at night, neon lights, rain"
- "Majestic lion in savannah sunset, photorealistic"
- "Steampunk library with floating books"

## Troubleshooting
| Issue | Solution |
|-------|----------|
| Authentication errors | Verify HF token is valid |
| CUDA out of memory | Use smaller model (SD 1.5) |
| Slow generation | Ensure GPU is selected |
| Blurry images | Make prompts more detailed |

## License
This notebook is provided under the [MIT License](LICENSE). Model weights are subject to Hugging Face's [model licenses](https://huggingface.co/models).

---
> **Note**: First execution may take 2-5 minutes for model download.  
> Generated images may be subject to content restrictions.
