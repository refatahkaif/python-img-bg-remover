# 🖼️ Image Background Remover (Python)

## ✅ Requirements
- Python 3.7 or newer
- pip

## 📦 Install
```bash
pip install rembg
# If you get an error about onnxruntime, run:
pip install onnxruntime
```

## 🚀 Usage
1. Put your image in the same folder and name it `cl.jpg`
2. Run the script:
```bash
python img-bg-remover.py
```

## 🧾 Script (img-bg-remover.py)
```python
from rembg import remove
from PIL import Image

input_path = 'cl.jpg'
output_path = 'output.png'

input = Image.open(input_path)
output = remove(input)
output.save(output_path)
```

## 📁 Output
A new image called `output.png` will be created with the background removed.
