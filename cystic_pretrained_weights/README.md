# ctstic_pretrained_weighted
This weight is a weight file that we trained ourselves to segment pancreatic cystic tumors. After customizing Task_069, inference can begin using the nnunet (v1) framework.
## Checkpoint
Cystic: Task069_Pancreas.rar (In Releases)

Solid: Use the nnUnet(V1) Pretrained Task007


After decompressing, replace the model weights.
## Usage Examples
nnUNet_predict \\
  -i "input folder" \\
  -o "output folder" \\
  -t Task069_Pancreas \\
  -m 3d_fullres \\
  -tr nnUNetTrainerV2 \\
  -p nnUNetPlansv2.1 \\
  -f 4

