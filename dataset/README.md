This project utilizes the following datasets for training and evaluating the Adversarial Residual U-Net model for building footprint detection:

1. SpaceNet Dataset

Source: SpaceNet on AWS | Kaggle

Description:

1.High-resolution satellite imagery (30–50 cm/pixel) with annotated building footprints.

2.Covers diverse cities (e.g., Vegas, Paris, Shanghai) with urban challenges like shadows, occlusions, and varying building densities.

3.Includes multi-spectral (RGB + PAN) and SAR data in some versions.


Labels: Polygon masks (GeoJSON) for building footprints.

Preprocessing:

1.Converted GeoJSON to binary masks (PNG) for segmentation.

2.Patched into 256×256 tiles for model input.


2. Manchester Building Detection Dataset

Source: Kaggle

Description:

1.Aerial imagery (0.5m resolution) of Manchester, UK, with labeled building footprints.

2.Focuses on dense urban and suburban areas, useful for testing model generalizability.

Labels: Binary masks (PNG) or shapefiles.

Preprocessing:

1.Resized to 512×512 pixels.

2.Augmented with rotations/flips to address class imbalance.


3. Drone Footage (Optional)
Source: Custom quad-type drone captures.

Purpose:

1.Augments training with dynamic perspectives and lighting conditions.

2.Enhances robustness to real-world occlusions (e.g., trees, vehicles).

Links for the datsets are :

1.https://drive.google.com/drive/folders/1M37GNOwjIggxbSZj1WWaeq2mp0bU6kOQ?usp=drive_link

2.https://drive.google.com/drive/folders/1DoM_fWSnJoOXf7aIWbdxXk2lnd_1eQnh?usp=drive_link
