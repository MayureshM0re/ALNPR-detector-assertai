# ALNPR Detector — YOLOv8 Model + Demo Videos

This repository runs a YOLO-based automatic license plate (ALPR) detector using the provided PyTorch model and demo videos.

Files in this workspace
- Model: [registration_plate.pt](registration_plate.pt)  
- Demo videos: [car2.mp4](car2.mp4)  
- Example output: [output_video.mp4](output_video.mp4)  
- Main runner script: [main.py](main.py) — uses the variables [`BASE_DIR`](main.py), [`model_path`](main.py), [`video_path`](main.py) and [`output_path`](main.py) and loads the model via the [`model`](main.py) symbol.

Google Drive with model & videos:
https://drive.google.com/drive/folders/1KSJ3uCjjQ5wlnUEHrYF1KnyTXZ70I-Jx?usp=drive_link

Quick setup

1. Create a virtualenv (recommended)
   - python3 -m venv .venv
   - source .venv/bin/activate

2. Install dependencies
   - pip install -U pip
   - pip install ultralytics torch opencv-python

Run the detector

- By default the script reads the paths set in [main.py](main.py):
  - model file: [`model_path`](main.py) -> points to [registration_plate.pt](registration_plate.pt)
  - input video: [`video_path`](main.py) -> points to  [car2.mp4](car2.mp4)
  - output video: [`output_path`](main.py) -> writes [output_video.mp4](output_video.mp4)

Example:
```sh
python [main.py]
