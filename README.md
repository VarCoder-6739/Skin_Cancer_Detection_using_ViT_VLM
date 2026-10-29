# Explainable Skin Cancer Detection using Hybrid Attention Vision Transformers (HAVT) and a
Vision Language Model 

## 📍
- Developed a Hybrid attention framework for seven-class skin-lesion classification using HAM10000 (10,015 images),
investigating pretrained ViT, Swin Transformer, DeiT and BEiT backbones.
- Evaluated attention-map fusion and reduction from 100 to 49, 28, and 7 maps, resulting in seven class-associated
maps; 92.62% accuracy based on an 80:20 train-test split.
- Generated attention heatmaps and integrated LlAMA 3.2 Vision Instruct (VLM) to provide text-based explanations
using original image, predicted class and attention maps; focused on misclassifications with visually similar and
under-represented classes.


## 💻Framework/Technology/Tools
- Python, PyTorch
- Vision-Language Models (VLMs), Hugging Face Transformers
-  Jupyter Notebook, Google Colab, Kaggle
- Vision Transformer(ViT), Swin Transformer, DeiT, BEiT

## 📁 Dataset
- HAM10000 Dataset


## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/VarCoder-6739/Skin_Cancer_Detection_using_ViT_VLM.git
cd Skin_Cancer_Detection_using_ViT_VLM
```

### 2. Create a Virtual Environment

**Windows (PowerShell):**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

**Linux / macOS:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
python -m pip install --upgrade pip
pip install torch torchvision
pip install transformers timm scikit-learn numpy pandas matplotlib pillow jupyter notebook ollama
```

For GPU-enabled PyTorch, choose the appropriate installation command for your system from the [official PyTorch installation guide](https://pytorch.org/get-started/locally/).

### 4. Set Up Llama 3.2 Vision

Install [Ollama](https://ollama.com/download), then download the vision model:

```bash
ollama pull llama3.2-vision
```

Ensure Ollama is running before generating explanations with the Vision-Language Model.

### 5. Download the Dataset

Download the HAM10000 dataset and configure the dataset path in the relevant notebook or Python script.

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells in sequence.
