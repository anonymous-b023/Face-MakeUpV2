# Face-MakeUpV2 🎨
## Demo

https://github.com/user-attachments/assets/a293827b-8922-4ac4-9978-99064ebaa9fe

## Model&Dataset

<img width="1098" height="895" alt="image" src="https://github.com/user-attachments/assets/fba427c6-5d87-463e-95f0-b3296bbd4943" />

## Results
### FaceCaption
| Model | CLIP-T ↑ | VLMScore↑ | Attr↑ | CLIP-I↑ | DINO↑ | FaceSim↑ | FID↓ | LPIPS↓ | Pose-RMSE↓ | Light-RMSE↓ |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Ipadapter-Faceid (2023) [37] | 25.1882 | 86.4300 | 3.9100 | 0.6440 | 0.5651 | 0.6042 | 122.9359 | 0.6788 | 0.1966 | 0.2181 |
| InstantID (2024) [33] | 25.6051 | 47.0000 | 3.5400 | 0.5107 | 0.4186 | 0.4495 | 126.3945 | 0.6647 | 0.1210 | 0.2945 |
| PhotoMaker (2024) [23] | **25.9190** | 72.3500 | 3.6900 | 0.5696 | 0.4578 | 0.1811 | 114.6484 | 0.6886 | 0.2308 | 0.2882 |
| MasterWeaver (2024) [34] | 25.7518 | 58.1000 | 3.7000 | 0.6052 | 0.5567 | 0.3564 | 106.7198 | 0.6828 | 0.2156 | 0.2253 |
| FaceMakeup (2025) [7] | 24.0256 | **88.3700** | 4.4000 | 0.7513 | 0.7219 | 0.7361 | 99.9833 | 0.6164 | 0.0947 | 0.1441 |
| Ours | 23.3556 | 84.2100 | **5.9000** | **0.7709** | **0.7857** | **0.7568** | **90.0322** | **0.5627** | **0.0907** | **0.1176** |
### Unsplash
| Model | CLIP-T ↑ | VLMScore↑ | Attr↑ | CLIP-I↑ | DINO↑ | FaceSim↑ | FID↓ | LPIPS↓ | Pose-RMSE↓ | Light-RMSE↓ |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Ipadapter-Faceid (2023) [37] | 25.2155 | 89.0600 | 4.4500 | 0.7649 | 0.6581 | 0.6534 | 102.9820 | 0.6554 | 0.2319 | 0.2363 |
| InstantID (2024) [33] | 25.9059 | 47.2200 | 3.2900 | 0.5279 | 0.4270 | 0.4360 | 143.1719 | 0.6852 | 0.1357 | 0.3237 |
| PhotoMaker (2024) [23] | 26.2755 | 75.0400 | 3.6600 | 0.6550 | 0.5170 | 0.2051 | 113.6866 | 0.6905 | 0.2641 | 0.3119 |
| MasterWeaver (2024) [34] | **26.7802** | 67.3900 | 4.2900 | 0.6363 | 0.5925 | 0.2980 | 113.0527 | 0.6919 | 0.2465 | 0.2662 |
| FaceMakeup (2025) [7] | 24.7941 | **91.0000** | 4.7100 | 0.7334 | 0.7192 | 0.6408 | 116.8287 | 0.6369 | 0.1003 | 0.1661 |
| Ours | 24.1836 | 88.6800 | **5.5100** | **0.7819** | **0.7893** | **0.7220** | **113.3948** | **0.5957** | **0.0448** | **0.1176** |

## Installation


1. Clone the repository:
```bash
git clone https://github.com/your-repo/Face-MakeUpV2.git
cd Face-MakeUpV2
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Download pretrained models (see Model Setup section)

## Model Setup

### Required Models:
- Base diffusion model (e.g., Realistic_Vision_V4.0)
- CLIP vision encoder
- Face recognition model
- Trained IP-Adapter weights

Please refer to the documentation for detailed model setup instructions.

## Usage

### Web Demo
```bash
python demo/demo_v5/web_demo.py
```

### Training
```bash
bash train/mask/lora/train_v5.sh
```

## Project Structure

```
Face-MakeUpV2/
├── train/              # Training scripts
├── models/             # Model architectures
├── dataset/            # Dataset processing
├── utils/              # Utility functions
├── demo/               # Demo applications
└── examples/           # Usage examples
```

