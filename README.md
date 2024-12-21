# Visual Model Distillation Project

This repository contains code for generating student models based on pre-trained teacher models. We explored 6 different methods to distill knowledge from teacher models to student models. The teacher models used in this project include(all the following models are retrived from their public repository):

- **CLIP**: Vision-Language Model (VLM)
- **BLIP**: Vision-Language Model (VLM)
- **BEIT**: Vision-Only Model
- **DINO**: Vision-Only Model

## Project Structure

The experiments of the project are divided into 2 sets:
1. **VLM-Based Experiments**: Conducted using CLIP and BLIP.
2. **Vision-Only Experiments**: Conducted using BEIT and DINO.

### Directory Organization
- **COCO-2017 Folder**: Contains all the files for student models generated from VLM teacher models (CLIP and BLIP).
- **TinyImageNet Folder**: 
  - Files with the dataset name are for downloading and preparing the TinyImageNet dataset.
  - Other files correspond to student models generated from vision-only teacher models (BEIT and DINO).

Each method corresponds to one file in each folder, making it easy to identify and run specific experiments.

## How to Run the Code

1. **Open the Corresponding File**:
   - Navigate to the relevant folder (`COCO-2017` for VLM models or `TinyImageNet` for vision-only models).
   - Select the file for the method you want to run.

2. **Prepare the Checkpoint Folder**:
   - Create a checkpoint folder with the name specified in the corresponding Jupyter notebook.
   - This folder is required to save and retrieve training checkpoints.

3. **Run the Code**:
   - Open the Jupyter notebook in your preferred environment, make sure the cuda is accessible.
   - Execute each code block in order.
   - Wait for the results to be generated.

## Notes

- Ensure that all required dependencies (e.g., PyTorch, torchvision, transformers) are installed in your environment before running the code.
- The output of each experiment, including training logs and student model checkpoints, will be saved in the specified checkpoint folder.
- Each experiment is self-contained within its respective Jupyter notebook, making it easy to replicate and analyze.
