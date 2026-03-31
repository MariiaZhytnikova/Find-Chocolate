# Object Tracking (Optical Flow)

Task from the **IT-Jim Computer Vision course**.

Goal: detect the target in the first frame using ORB keypoints (matched with a marker image), then track it through the video with Lucas-Kanade optical flow.

## Files

- `Optical_flow.ipynb` - main notebook solution
- `ORB_Opt_Flow.avi` - output tracking video

## Input -> output example

| Item | Example |
| --- | --- |
| Marker (input image) | ![marker](../source/marker.jpg) |
| Input video | [`../source/find_chocolate.mp4`](../source/find_chocolate.mp4) |
| Output video | [`ORB_Opt_Flow.avi`](ORB_Opt_Flow.avi) |

### Result preview

![Optical flow example](example_frame.png)

## Pipeline summary

1. Load marker image and source video.
2. Detect ORB keypoints/descriptors on marker and first frame.
3. Match marker-to-frame points with BFMatcher.
4. Initialize tracked points from matched keypoints.
5. Track points with `cv2.calcOpticalFlowPyrLK`.
6. Draw a bounding rectangle around tracked points and write output frames.

## Run

Open and run `Optical_flow.ipynb` from this folder.  
The notebook uses:

- `../source/marker.jpg`
- `../source/find_chocolate.mp4`

