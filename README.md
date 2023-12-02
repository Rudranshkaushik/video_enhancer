# Video Upscaling with OpenCV

This Python script uses the OpenCV library to upscale a video by a factor of 2. It reads a video file, upscales each frame using linear interpolation, and writes the upscaled frames to a new video file.

## Prerequisites

Make sure you have the following dependencies installed:

- OpenCV: `pip install opencv-python`

## Usage

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/your-repository.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd your-repository
    ```

3. **Replace the `input_video_path` variable with the path to your input video file:**

    ```python
    input_video_path = '/path/to/your/input/video.mp4'
    ```

4. **Run the script:**

    ```bash
    python upscale_video.py
    ```

5. **Check the output video:**

    The upscaled video will be saved as `output_video.avi` in the project directory.

## Customize

Feel free to customize the script based on your requirements. You can modify the input video path, output video path, or adjust the upscaling factor.

```python
# Input video file path
input_video_path = '/path/to/your/input/video.mp4'

# Output video file path
output_video_path = 'output_video.avi'

# Upscaling factor
scaling_factor = 2

# ...

# Upscale the frame using linear interpolation
upscaled_frame = cv2.resize(frame, (width * scaling_factor, height * scaling_factor), interpolation=cv2.INTER_LINEAR)

# ...
