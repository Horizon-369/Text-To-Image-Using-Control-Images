# Text-to-Image Generation with Control Images 

## Overview
This project utilizes pretrained models and Stable Diffusion techniques to generate images from textual prompts while incorporating control images, such as depth maps, to guide the generation process. The process involves converting images into suitable control formats and then passing both the control image and prompt to the StableDiffusionAdapterPipeline for image generation.

## Requirements
- Python 3.6 or higher
- PyTorch
- Transformers library
- Hugging Face 

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/your_repository.git
   ```

2. Install the required dependencies:
   ```bash
   !pip install huggingface-hub
   !pip install diffusers accelerate transformers
   !pip install git+https://github.com/huggingface/diffusers
   ```

## Usage
1. **Prepare Control Images**:
   Input image:
   
   ![image](https://github.com/Horizon-369/Text-To-Image-Using-Control-Images/assets/124186027/90e5d410-d8bc-4be5-a5f4-28ce6711c3e5)


3. **Create Your Color Palette**:
   Convert control images, such as depth maps, into the appropriate format for controlling the image generation process.
   ```bash
   from PIL import Image
    color_palette = image.resize((8, 8))
    color_palette = color_palette.resize((512, 512), resample=Image.Resampling.NEAREST)
   ```
   Color Palette:
   
   ![image](https://github.com/Horizon-369/Text-To-Image-Using-Control-Images/assets/124186027/25ce8944-453e-4978-a886-0a8d84828988)


5. **View Results**:
   The text prompt used.
   ```bash
    "At night, glowing coconut trees in front of the beach"
   ```
   Output Image:
   
   ![image](https://github.com/Horizon-369/Text-To-Image-Using-Control-Images/assets/124186027/3321f3c1-c36b-400d-b6a0-a2dca1a2ce60)



## Citation
If you use this code or the pretrained models in your research, please cite the relevant papers and repositories.

## Acknowledgements
This project builds upon the work of several research papers and repositories. We acknowledge the contributions of the authors and developers.

## References
- Hugging Face: [HuggingFace]([https://github.com/huggingface/datasets](https://huggingface.co/docs/diffusers/en/api/pipelines/stable_diffusion/adapter))

--- 
