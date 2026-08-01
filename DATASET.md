# Dataset setup

The image dataset is deliberately excluded from this repository.

The original project used the public chest X-ray pneumonia dataset commonly distributed through Kaggle, with experiments that also considered extra normal chest X-rays. Before reproducing the project, review the current dataset licence and usage conditions at the source.

Place the images outside the Git repository and use this layout:

```text
chest_xray/
├── train/
│   ├── NORMAL/
│   └── PNEUMONIA/
├── val/
│   ├── NORMAL/
│   └── PNEUMONIA/
└── test/
    ├── NORMAL/
    └── PNEUMONIA/
```

Then set the notebook's `DATA_ROOT` variable to the `chest_xray` directory.

Do not commit:

- raw chest X-rays;
- patient-identifiable material;
- Google Drive paths;
- trained model files;
- large ZIP archives;
- secret keys or tokens.
