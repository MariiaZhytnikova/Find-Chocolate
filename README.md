# CV Tracking Tasks (IT-Jim Course)

This repository section contains two related tasks from the **IT-Jim Computer Vision course**:

- **Optical Flow object tracking** (`flow/`)
- **Homography-based marker detection** (`homography/`)

Both tasks use the same source assets from `source/`.

## Structure

- `flow/` - ORB-initialized Lucas-Kanade tracking notebook, output video, and preview
- `homography/` - ORB + BFMatcher + RANSAC homography notebook, output video, and preview
- `source/` - shared input files (`marker.jpg`, `find_chocolate.mp4`)

## Inputs

- Marker image: `source/marker.jpg`
- Source video: `source/find_chocolate.mp4` (will be added later)

## Outputs

- Optical flow result: `flow/ORB_Opt_Flow.avi`
- Homography result: `homography/ORB_Homography.avi` (will be added later)

## Read task details

- Flow task README: [`flow/README.md`](flow/README.md)
- Homography task README: [`homography/README.md`](homography/README.md)

