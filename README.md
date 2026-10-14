# MotionFit AI

Responsive webcam movement game prototype using MediaPipe Pose Landmarker.

## Features
- Live camera preview and pose landmark overlay
- Balance Hold, Side Step, and Squat Challenge missions
- Score, rep counter, mission timer, balance meter, and live coaching feedback
- Responsive UI for desktop, tablet, and iPad
- Video is processed in the browser and is not uploaded by this app

## Run locally
Camera access requires HTTPS or localhost.
1. Open the project folder in VS Code.
2. Use the Live Server extension to open `index.html`, or run `python -m http.server 8000` from this folder.
3. Visit `http://localhost:8000` on the same computer.

## Publish for iPad with GitHub Pages
1. Create a GitHub repository such as `motionfit-ai`.
2. Upload `index.html`, `style.css`, `app.js`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/(root)`, then save.
5. Open the published HTTPS address in Safari on your iPad and allow camera access.

## Notes
- An internet connection is needed to load MediaPipe and the pose model from their CDNs.
- Good lighting and a stable camera improve tracking.
- Pose-based rep detection is a lightweight prototype and may miscount based on angle, clothing, lighting, or body visibility.
- This is an educational project, not a medical device or professional fitness assessment. Stop if you feel pain or dizziness.

## Technology
HTML, CSS, JavaScript ES modules, MediaPipe Tasks Vision Pose Landmarker.
