# Clothing Detection
 _Thesis 2023_

 This repository stores the source code for a YOLOv8 Model that is trained to detect suitable classes. The model uses the [YOLOv8](https://github.com/ultralytics/ultralytics) architecture and the [Deepfashion2](https://github.com/switchablenorms/DeepFashion2) dataset. CUDA is required to run file.

# How To Run

 1. Make sure that your opencv installation is correct for the system. If you are on windows, use ``opencv`` but if you're working on a Linux system, use ``opencv-headless`` instead.
 2. To use the model, script ``9_camera.ipynb`` is what you need.
 3. Model is provided in the folder ``11-24-2023-100epchs-nopre/weights/``, pick whether you want to use ``best.pt`` or ``latest.pt``. Change model settings in ``model_path``.
 4. Similar to the model settings, the ``args.yaml`` file is also provided in the ``11-24-2023-100epchs-nopre`` folder. Change the yaml settings in ``args_path``.
 5. Run ``9_camera.ipynb`` as a python notebook. To quit, press ``Q``

Below are the dependencies and hardware used for the code:
## Python Libraries
- Anaconda Navigator
- Jupyter Notebook
- Python 3.11.3
- Ultralytics 8.0.23
- Torch 2.0.1+cu118
- Torchvision 2.0.1+cu118
- opencv 4.7.0.72
- scikit-learn 1.2.2.
- shapely 2.0.2
- pybboxes 0.1.6
- pydot 3.0.9
- pyzipper 0.3.6
- gdown 4.7.1
- tdqm 0.4.6
- albumentations 1.3.1

## Hardware
- Windows 10 OS
- Ram 16 GB
- Processor Intel(R) Core(TM) i7-8700k CPU @ 3.70GHz
- NVIDIA GeForce GTX1080 Ti

Following the training process, the following are the metrics:

|           | Micro Average | Macro Average |
|-----------|---------------|---------------|
| Precision | 53.5%         | 48.9%         |
| Recall    | 44.6%         | 58.6%         |
| f1-score  | 48.6%         | 53.3%         |
