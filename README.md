# carracing_fullmap
Variant of OpenAI Gym CarRacing environment with full map observation.

## Environment Description

This environment is a modified version of the [CarRacing environment](https://www.gymlibrary.dev/environments/box2d/car_racing/) from OpenAI Gym. By default, the rendered images show a full map
of the track instead of a limited FOV view. It also includes an offline rendering feature, which produces a simulated rendered image given a particular road polygon (defining the contours of the road) and car state.

Other changes to `env.render()`
- Keeps a fixed zoom
- Keep a fixed view of the track (doesn't scroll)
- Doesn't change angle of view as car rotates
- Doesn't render the indicators (speed, etc.)

## Requirements
- Gym 0.21.0

## Usage
To test the environment using human keyboard inputs, simply run:
```
python fullmap_carracing.py
```