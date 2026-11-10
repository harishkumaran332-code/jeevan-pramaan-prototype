# Jeevan Pramaan — plain-language rejection prototype

A lo-fi functional prototype built for a Design Thinking (Human-Centred Design
Process) assignment, demonstrating **Idea #1** from the Idea Selection Matrix:
replacing the generic "Verification Failed" message with a specific,
plain-language reason, for an elderly user (persona: Viswan, 82) with limited
digital experience submitting an annual Jeevan Pramaan digital life certificate.

## What it demonstrates

- Uses the device's real camera (browser permission required) and measures the
  live brightness of the feed when **Take Photo** is tapped.
- Too dark -> "Photo too dark"; too bright -> "Too much glare"; otherwise it
  succeeds (with an occasional "Face not fully visible" to show all reasons).
  Each rejection gives one plain-language reason and one instruction, instead
  of a generic failure message. If no camera is available it falls back to a
  simulated attempt.
- An expandable **Viswan's experience** panel shows the Says / Thinks / Feels /
  Does from the Empathy Map that motivates the design.
- A **Compare with old version** toggle switches to today's actual rejection
  screen ("Verification Failed" / "Retry") for a side-by-side demo.
- Large text, high contrast, and big tap targets, matching the persona's needs.

This is a static, front-end-only demo — it is not connected to any real
authentication system and does not collect or transmit any data.

## Run it

Camera access needs `localhost` or HTTPS (it works on GitHub Pages). Serve the folder with any static
file server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Project context

Built as part of Experiment 3 (Ideation and Prototyping), Human-Centred
Design Process, Faculty of Engineering and Technology.
