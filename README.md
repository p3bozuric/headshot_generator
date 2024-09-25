# No-Code Headshot Generator

![grid](assets/headshot_generator.png)

This project provides tools with easy access for fine-tuning and using a professional headshot generator based on the FLUX.1-dev model. It consists of two main components:

1. A training notebook for fine-tuning the model
2. An inference notebook for generating headshots using the fine-tuned model

## Prerequisites

- A Google account with access to Google Colab & A100 GPU
- Sufficient Google Drive space for storing the model and generated images
- Hugging Face token for accessing the FLUX.1-dev model.

## Usage

### Training Notebook

[Open In Colab](https://colab.research.google.com/github/p3bozuric/headshot_generator/blob/main/headshot_generator_finetuning.ipynb)

1. Open the training notebook by clicking "Open In Colab" above.
2. Ensure you're using a runtime with a GPU (preferably A100).
3. Mount your Google Drive.
4. Set up your project configuration like file outputs,..
5. Configure training parameters such as batch size, number of steps, learning rate, etc.
6. Run the cells to start the training process.

### Inference Notebook

[Open In Colab](https://colab.research.google.com/github/p3bozuric/headshot_generator/blob/main/headshot_generator_inference.ipynb)

1. Open the inference notebook by clicking "Open In Colab" above.
2. Ensure you're using a runtime with a GPU (preferably A100).
3. Mount your Google Drive.
4. Load your fine-tuned model.
5. Set up your inference configuration, including:
   - Prompt
   - Number of images to generate
   - Image dimensions
6. Run the cells to generate headshots.
7. For additional generations switch up configuration in last cell and rerun it.

## Model Information

This project uses the FLUX.1-dev model as its base. FLUX is a text-to-image model designed for high-quality image generation.

## License

This project extends from the LICENSE-FLUX1-dev, which can be found [here](https://github.com/black-forest-labs/flux/blob/main/model_licenses/LICENSE-FLUX1-dev).

Key points of the license include:

- The model can be used for commercial and non-commercial purposes.
- Redistribution of the original or modified model is allowed under certain conditions.
- There's no warranty provided with the model.

Please refer to the full license for complete terms and conditions.

## Acknowledgments

- Black Forest Labs for the FLUX.1-dev model
- lucataco for his cog-ai-toolkit

## Disclaimer

This tool is designed to generate professional headshots. Users are responsible for ensuring they have the right to use and potentially distribute any images generated using this tool, especially if they contain likenesses of real individuals.

## Support

For issues related to the code in these notebooks, please open an issue in this repository. For questions about the FLUX model itself, please refer to the [FLUX GitHub repository](https://github.com/black-forest-labs/flux).
