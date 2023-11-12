## Object Detection in Video using YOLOv8 🚀

This repository contains a Python script for performing object detection in a video using YOLOv8. The script uses the OpenCV library to read and write videos, and a YOLOv8 model for object detection.

### Prerequisites 🛠️

Make sure you have the following dependencies installed:

- Python 🐍
- OpenCV 📸
- YOLOv8 model file (e.g., `yolov8m_custom.pt`) 🤖

### Setup 🚧

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/yourrepository.git
   cd yourrepository
   ```

2. **Create a directory named `videos` in the root of the repository and place your input video file (e.g., `cananddog.mp4`) inside it.**

3. **Download the YOLOv8 model file (e.g., `yolov8m_custom.pt`) and place it in the appropriate directory (e.g., `./runs/detect/train/weights/`).**

### Usage 🚀

Edit the script to set the correct file paths:

```python
VIDEOS_DIR = os.path.join('.', 'videos')
video_path = os.path.join(VIDEOS_DIR, 'cananddog.mp4')
video_path_out = '{}_out.mp4'.format(video_path)
model_path = os.path.join('.', 'runs', 'detect', 'train', 'weights', 'yolov8m_custom.pt')
```

Adjust the `threshold` variable if needed. This controls the confidence threshold for object detection.

### Run ▶️

Execute the script by running the following command:

```bash
python your_script_name.py
```

Replace `your_script_name.py` with the actual name of your Python script.

### Output 🎥

The script will generate an output video file (`cananddog_out.mp4`) in the same `videos` directory with detected objects framed and labeled.

### Cleanup 🧹

Ensure to close the video display window after the script finishes executing.

```bash
cv2.destroyAllWindows()
```

Feel free to customize the script according to your requirements. For more details about YOLOv8, refer to the [YOLOv8 GitHub repository]([https://github.com/ultralytics/yolov5](https://github.com/ultralytics/ultralytics)).

---

Feel free to adjust the emojis or add more based on your preferences!
