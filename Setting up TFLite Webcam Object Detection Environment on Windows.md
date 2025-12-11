### Setting up TFLite Webcam Object Detection Environment on Windows

---

1. **Open Anaconda Prompt**

2. **Create a new environment with Python 3.10**
```bash
conda create -n tflite1 python=3.10
conda activate tflite1
```

3. **Install required packages**
```
python -m pip install numpy==1.23.5
python -m pip install tensorflow==2.13.0
python -m pip install opencv-python==4.7.0.72
python -m pip install playsound==1.3.0

# Optional: Install TFLite runtime if needed
python -m pip install tflite-runtime
```

4. **Verify installation**
```bash
python
```
```python
import cv2
import numpy as np
import tensorflow as tf

print(cv2.__version__)   # should be 4.7.0
print(np.__version__)    # should be 1.23.5
print(tf.__version__)    # should be 2.13.0
exit()
```

5. **Run your TFLite script**
```bash
cd C:\Users\scrim\tflite-venv
python TFLite_detection_webcam.py --modeldir=custom_model_lite
```

---

Everything should now run without errors.

