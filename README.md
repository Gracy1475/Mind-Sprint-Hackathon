# Computer Vision Exercise Form Coach

Real-time exercise form analysis via your webcam using OpenCV and MediaPipe. Supports squats, pushups, and planks with rep counting and actionable feedback cues.

## Quick Start

1. Install Python 3.9+.
2. Create a virtual environment (recommended).
3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the app (choose exercise: squat | pushup | plank | jogging | walking | situp | singleleg | jumpingjacks | lunge | bicepcurl | shoulderpress):

```bash
python app.py --exercise squat
```

Press `q` to quit. Press `e` to cycle exercises at runtime.

## Features

- Real-time pose detection with MediaPipe
- Rep counting for squats, pushups, sit-ups
- Step counting and cadence/pace for jogging and walking (gated by arm swing)
- Balance scoring for single-leg stand
- Continuous alignment scoring for planks
- Multi-person mode with per-person IDs and counts (`--multi`)
- Idle detection (`--idle`) shows exercise steps after 5s; raise right/left hand to switch
- On-screen feedback cues and form highlights

## Notes

- Lighting and camera angle affect accuracy. Keep your full body visible.
- This tool is for educational feedback and not a medical device.


