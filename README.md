# Eyes-Open Terms & Conditions Scroller

A fun browser demo that **prevents scrolling** through a Terms & Conditions page unless your eyes are open.  
It uses **[MediaPipe Face Mesh](https://developers.google.com/mediapipe/solutions/vision/face_mesh)** for real-time facial landmark detection, runs **entirely on-device** in your browser, and does **not send video data anywhere**.

## Features
- Locks mouse wheel & touch scroll until eyes are detected open.
- Fake Terms & Conditions text for testing.
- Lightweight — pure HTML, CSS, and JavaScript.
- No build tools or backend required.
- Uses **MediaPipe Face Mesh** + **Camera Utils** via jsDelivr CDN.

  
## How It Works
1. The page loads your webcam feed (with permission).
2. MediaPipe Face Mesh detects facial landmarks each frame.
3. A simple **Eye Aspect Ratio (EAR)** is calculated to determine if your eyes are open.
4. If eyes are open for a few consecutive frames → scrolling is unlocked.
5. If eyes close → scrolling is locked again.

## Requirements
- Any modern browser with webcam access (Chrome, Edge, Firefox).
- Internet connection (to load MediaPipe scripts from CDN).
- User consent for webcam access.

## Usage
1. **Clone this repo** or download the `index.html` file.
2. Open `index.html` in your browser.
3. Allow webcam access.
4. Keep your eyes open to scroll through the Terms & Conditions.
