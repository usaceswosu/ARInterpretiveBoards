# AR Interpretive Boards

This project is a browser-based augmented reality experience built with A-Frame and AR.js. When a supported marker is detected by your camera, a matching video is rendered on top of that marker.

## What This Project Does

- Uses your webcam (or phone camera) to detect pattern markers.
- Displays one of four videos on top of the detected marker.
- Plays video while marker is visible and pauses when marker is lost.

## Project Structure

- index.html: Main AR scene, marker setup, and video logic.
- assets/*.patt: Marker pattern files used for detection.
- assets/*.mp4: Videos displayed on matching markers.

## Requirements

- A modern browser (Chrome, Edge, or Firefox).
- Camera access permission enabled.
- HTTPS or localhost when running in environments that restrict camera access on plain HTTP.

## Quick Start

1. Clone or download this repository.
2. Open the folder in VS Code.
3. Run a local server from the project root.
4. Open index.html through that local server URL in your browser.
5. Allow camera permissions when prompted.

## Step-by-Step: How To View The Videos

1. Start a local web server in this folder.
	 - Example using Python:
		 - python -m http.server 8000
2. In your browser, go to:
	 - http://localhost:8000
3. When prompted, allow camera access.
4. Show one of the printed or on-screen marker patterns to the camera.
5. Hold the marker steady in good lighting.
6. The mapped video should appear on top of the marker and play automatically.
7. Move the marker out of view to pause the video.

## Marker To Video Mapping

- assets/marker.patt -> assets/asset.mp4
- assets/marker2.patt -> assets/ARBOARD PORTS and stuff.mp4
- assets/marker3.patt -> assets/Staircase Of Water Finished Video.mp4
- assets/hiro.patt -> assets/AR Board 3 FINAL.mp4

## Troubleshooting

- Camera does not start:
	- Check browser camera permissions.
	- Reload the page after allowing access.
- Marker not detected:
	- Improve room lighting.
	- Hold marker flat and fully visible.
	- Avoid blur by keeping the camera stable.
- Video not playing:
	- Confirm the video file exists in assets.
	- Open browser DevTools and check for missing file errors.
	- Try another browser if autoplay policy blocks playback.

## Editing Content

- To replace a video, keep the same filename in assets or update the matching src value in index.html.
- To change which marker triggers a video, update the marker url and a-video src pairing in index.html.
- To add another AR board, duplicate an existing marker block in index.html and connect it to a new video and .patt file.

## Credits

This project appears to be based on prior AR Interpretive Boards work and has been preserved for capstone use.

Current Group of Spring 26:

Aaryn Minyard
Casey Zachary
Dillon Martinez
Ethan Brandy
Nicolas Hill
Tyler Kirsch