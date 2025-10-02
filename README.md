# Face-MakeUpV2 🎨
## Demo

https://github.com/user-attachments/assets/a293827b-8922-4ac4-9978-99064ebaa9fe

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

