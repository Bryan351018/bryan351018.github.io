---
layout: single
needs_math: true # This page needs math typesetting
# If you need chem typesetting, use needs_chem: true
toc: true
toc_label: "Quick jump"
toc_icon: "file-alt"
sidebar:
  nav: "projects"

permalink: /projects/desmos/
---

# Desmos Projects

## DeSyne
[DeSyne](https://www.desmos.com/calculator/twlat5kmup) (pronounced like "design") is a synthesizer that I made for the [2023 Global Math Art Contest](https://www.desmos.com/art-2023).
It:
- can play all 4 fundamental waveforms: sine, triangle, square, sawtooth.
  - For the last 3 waveforms, you can choose how many sine waves are used to reconstruct the waveform, functioning like a low-pass filter.
- has a fully-functional ADSR envelope
- has a volume knob
- has a note length knob
- has 11 octaves of range, and you can play 2 octaves simultaneously
- supports polyphony, up to 312 notes theoretically
- has draggable controls for everything, **including the keyboard**

## Fractals
As Desmos now natively supports [Recursion](https://help.desmos.com/hc/en-us/articles/25917735966989-Recursion) and [Complex Numbers](https://help.desmos.com/hc/en-us/articles/31103542590733-Complex-Numbers), making fractals has become *easier than ever*. Here are a few that I made:
- [Julia Set](https://www.desmos.com/calculator/zm2qtvihoc)
- [Mandelbrot Set](https://www.desmos.com/calculator/x9whrwtwqx)
- [Newton Fractal](https://www.desmos.com/calculator/nkzdrwtnhu)
  - Takes a while to load
  - This fractal is for \\( f(z) = z^3 - 1, \ z \in \mathbb{C} \\)

## Kinematics
Anything with moving things modelled after real-life classical kinematics.
- [Accelerating Object](https://www.desmos.com/calculator/tn45iczs6m)
  - Click the metronome icon to start the simulation.
  - Drag the red point around to accelerate the black circle according to its position.
  - There are different colored lines:
    - **Black** line = displacement
    - **Blue** line = velocity
    - **Red** line = acceleration
- [Spinning Object](https://www.desmos.com/calculator/sgaji4l0mo)
  - Drag the black point on the circle to resize it.
    - Resizing *does not change the speed* of the moving point, which should otherwise happen in real life.
  - Drag the orange point at the bottom to change the point's angular acceleration.
  - Click the purple bar below the orange point to reset the angular acceleration to 0.

## DesMoment
[DesMoment](https://www.desmos.com/calculator/u57xjpsbnv) is a stopwatch in Desmos.
- Click the metronome icon to start, and click it again to stop.
- Click the arrow to the left of \\( F_{init}() \\) in the expressions panel to reset the stopwatch.
